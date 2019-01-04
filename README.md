# Kick-Ass-App-WASD
Modified version of https://kickassapp.com/ that supports WASD.

To start destroying the web in retro space fashion you'll need to create a bookmark in your web browser with any name (e.g. "Kick Ass WASD") and the following cdn.jsdelivr.net alternative URL as JS files can't be loaded directly from GitHub (notes belows).
 
`javascript:var%20KICKASSVERSION='2.0';var%20s%20=%20document.createElement('script');s.type='text/javascript';document.body.appendChild(s);s.src='//cdn.jsdelivr.net/gh/michaelharper/Kick-Ass-App-WASD/kickass.js';void(0);`


# Why is this needed?

In 2013, GitHub started using X-Content-Type-Options: nosniff, which instructs more modern browsers to enforce strict MIME type checking. It then returns the raw files in a MIME type returned by the server, preventing the browser from using the file as-intended (if the browser honors the setting).

https://stackoverflow.com/questions/17341122/link-and-execute-external-javascript-file-hosted-on-github
