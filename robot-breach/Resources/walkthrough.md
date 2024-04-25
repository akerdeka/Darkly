Let's crawl the website to look for hidden folders
We used gospider with this command : ```./gospider -s http://127.0.0.1:8080 -o output -c 100 -d 0```
We can see two locations in [robots] : /whatever and /.hidden

Let's have a look at /whatever => There is a htpasswd so let's have a look inside
We have a root and a md5 password (qwerty123@)
As it's a Linux arch there is a /admin page so let's try those credentials here
GG we have our flag