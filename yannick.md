# Security Breaches reported by the community

## Access to JSON files

We can access to json files directly from the web interface, i.e. /data/users/phi&user.json

The fact that the index.php file is not in the root directory is a not a good practice. It is better to put it in the root directory and to use a .htaccess file to redirect all the requests to the index.php file.

## XSS

We can inject javascript code in proposition form, i.e. `<script>window.location='https://static.tvtropes.org/pmwiki/pub/images/punkd.jpg'</script>`

## CSRF

There is no protection against CSRF, the cookie and the token are not checked.

## Upload any type of file

We can upload any type of file, i.e. .exe file

## Use JQuery

Erk !
