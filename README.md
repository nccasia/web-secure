# web-secure
# ISO27001
##  Nullify Slow HTTP POST vulnerability
External Security Review Finding

The web server is possibly vulnerable to a "slow HTTP POST" Denial of Service (DoS) attack. This is an application-level DoS that consumes server resources by maintaining open connections for an extended period of time by slowly sending traffic to the server. If the server maintains too many connections open at once, then it may not be able to respond to new, legitimate connections. Unlike bandwidth consumption DoS attacks, the "slow" attack does not require a large amount of traffic to be sent to the server -- only that the client is able to maintain open connections for several minutes at a time. The attack holds server connections open by sending properly crafted HTTP POST headers that contain a Content-Length header with a large value to inform the web server how much of data to expect. After the HTTP POST headers are fully sent, the HTTP POST message body is sent at slow speeds to prolong the completion of the connection and lock up server resources. By waiting for the complete request body, the server is helping clients with slow or intermittent connections to complete requests, but is also exposing itself to abuse.
## Nullify Clickjacking - Framable  Page vulnerability
External Security Review Finding

The web page can be framed. This means that clickjacking attacks against users are possible. With clickjacking, an attacker can trick a victim user into clicking an invisible frame on the web page, thereby causing the victim to take an action they did not intend to take.
## Use of moment version 2.0 vulnerability
External Security Review Finding

CVE-2016-4055: moment versions below 2.11.2 are vulnerable to regular expression denial of service when user input is passed unchecked into moment.duration() blocking the event loop for a period of time.(https://github.com/moment/moment/issues/2936)
## Use of Bootstrap version 3.3.7 vulnerability
External Security Review Finding

The web application is using a JavaScript library that is known to contain at least one vulnerability. Attackers could potentially exploit the vulnerability in the JavaScript library. The impact of a successful exploit depends on the nature of the vulnerability and how the web application makes use of the library.
## Use of JQuery version 3.1.0 vulnerability
External Security Review Finding

The web application is using a JavaScript library that is known to contain at least one vulnerability. Attackers could potentially exploit the vulnerability in the JavaScript library. The impact of a successful exploit depends on the nature of the vulnerability and how the web application makes use of the library.
## Use of Angular version 1.5.9 vulnerability
External Security Review Finding

The web application is using a JavaScript library that is known to contain at least one vulnerability. Attackers could potentially exploit the vulnerability in the JavaScript library. The impact of a successful exploit depends on the nature of the vulnerability and how the web application makes use of the library.
## Sensitive form field has not  disabled autocomplete vulnerability
External Security Review Finding

An HTML form that collects sensitive information does not prevent the browser from prompting the user to save the populated values for later reuse. Autocomplete should be turned off for any input that takes sensitive information such as credit card number, CVV2/CVC code, U.S. social security number, etc. If the browser is used in a shared computing environment where more than one person may use the browser, then "autocomplete" values may be submitted by an unauthorized user.
## X-Frame-Options header is  not set vulnerability
External Security Review Finding

The X-Frame-Options header is not set in the HTTP response, meaning the page can potentially be loaded into an attacker-controlled frame. This could lead to clickjacking, where an attacker adds an invisible layer on top of the legitimate page to trick users into clicking on a malicious link or taking a harmful action. Without an X-Frame-Options response header, clickjacking may be possible. However, if the application properly uses the Content-Security-Policy "frame ancestors" directive, then modern web browsers would stop the page from being framed and prevent clickjacking.
## Path-relative stylesheet  import (PRSSI) vulnerability
External Security Review Finding

Relative URLs can be dangerous since browser may not determine the correct directory. If the HTML uses path-relative CSS links, it may be susceptible to path relative stylesheet import (PRSSI) vulnerabilities. This could allow an attacker to take advantage of CSS imports with relative URLs by overwriting their target file. An attacker may trick browsers into importing JavaScript or HTML code as a stylesheet. This has been shown to enable a number of different attacks, including cross-site scripting (XSS) and exfiltration of CSRF tokens.
# Remote and Local File Inclusion 
# Cross-Site Scripting (XSS)
# Cross-Site Request Forgery (CSRF)
# SQL Injection (SQLi)
# Command Injection
# OWASP Top 10 List
