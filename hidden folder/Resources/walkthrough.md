As this website turns on a linux arch there is a /etc/passwd file somewhere, maybe we can find something here
So start by http://localhost:8080/?page=/etc/passwd => nope
Let's add ```/../``` and see if we can find something
And here we go : http://localhost:8080/?page=/../../../../../../../etc/passwd => we have our flag