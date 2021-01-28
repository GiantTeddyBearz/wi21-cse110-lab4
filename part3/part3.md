# Part 3  
## DevTools - Debugging:
The bug was that it is appending both numbers as strings. To fix this, we can either parseInt or add unary + infront of getElementById to turn the value into a number.  Screenshot of fix under fix.png  
  
## DevTools - Network Tab  
1. citylots.json  
2. parts2.js  
3. 11.7 MB  
4. 69 ms  
5. Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/88.0.4324.104 Safari/537.36  
6. Apache  
7. Tue, 26 Jan 2021 22:14:13 GMT  
8. application/json  
9. `fetch('./citylots.json')`  