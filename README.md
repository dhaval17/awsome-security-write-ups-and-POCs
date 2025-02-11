## Awesome Security Write-Ups and POCs
> A curated list of delightful writeups and POCs

####  Not mine not yours, It's everyone's. Feel free to contribute.

![hacking-resource](https://github.com/dhaval17/hacking-resources/raw/assets/images/hacker.jpg)


#### Submitting new resource :
	
Please read the [Contribution Doc](/contribution.md)
#### Content

1. [Cross Site Scripting - XSS](https://github.com/dhaval17/awesome-writeups/blob/master/README.md#cross-site-scripting---xss)
2. [Cross Site Request Frogery - CSRF](https://github.com/dhaval17/awesome-writeups/blob/master/README.md#cross-site-request-frogery---csrf)
3. [Server Side Request Frogery - SSRF](https://github.com/dhaval17/awesome-writeups/blob/master/README.md#server-side-request-frogery---ssrf)
4. [Application/Business Logic](https://github.com/dhaval17/awesome-writeups/blob/master/README.md#applicationbusiness-logic)
5. [SQL Injection - SQLi](https://github.com/dhaval17/awesome-writeups/blob/master/README.md#sql-injection---sqli)
6. [InDirect Object Reference - IDOR](https://github.com/dhaval17/awesome-writeups/blob/master/README.md#indirect-object-reference---idor)
7. [Code Execution](https://github.com/dhaval17/awesome-writeups/blob/master/README.md#code-execution)
8. [Reverse Engineering](https://github.com/dhaval17/awesome-writeups/blob/master/README.md#reverse-engineering)
9. [DNS Related](https://github.com/dhaval17/awesome-writeups/blob/master/README.md#dns-related)
10. [Brute-force](https://github.com/dhaval17/awesome-writeups/blob/master/README.md#brute-force)
11. [Subdomain Takeover](https://github.com/dhaval17/awesome-writeups/blob/master/README.md#subdomain-takeover)
12. [Open URL Redirection](https://github.com/dhaval17/awesome-writeups/blob/master/README.md#open-url-redirection)
13. [XML Attacks](https://github.com/dhaval17/awesome-writeups/blob/master/README.md#xml-attacks)
14. [HTTP Request Smuggling Desync Attack](https://github.com/dhaval17/awesome-writeups/blob/master/README.md#http-request-smuggling-desync-attack)
15. [Research Papers](https://github.com/dhaval17/awesome-writeups/blob/master/README.md#research-papers)
16. [Miscellaneous](https://github.com/dhaval17/awesome-writeups/blob/master/README.md#miscellaneous)

#### Resource

##### Blogs/Write ups

###### Cross Site Scripting - XSS

1. [
XSS that existed at accounts.google.com](http://masatokinugawa.l0.cm/2013/06/accounts.google.com-utf-32-xss.html) - [@kinugawamasato](https://twitter.com/kinugawamasato)
2. [admin.google.com Reflected Cross-Site Scripting (XSS)](https://buer.haus/2015/01/21/admin-google-com-reflected-cross-site-scripting-xss/) - [@bbuerhaus](https://twitter.com/bbuerhaus) - Vulnerable `continue` parameter, `https://admin.google.com/mrzioto.com/ServiceNotAllowed?service=grandcentral&continue=javascript:alert(document.cookie);//`
3. [XSS-es in Google Caja](http://blog.bentkowski.info/2016/07/xss-es-in-google-caja.html) - [@SecurityMB](https://twitter.com/SecurityMB)
4. [Content Types and XSS: Facebook Studio](https://whitton.io/articles/content-types-and-xss-facebook-studio/) - [@fin1te](https://twitter.com/fin1te) - Client-side validation for content-type, Which then enables to pass `HTML/Javascript` to execute XSS
5. [Facebook XSS via Cross-Origin Resource Sharing](http://maustin.net/2010/07/06/facebook_html5.html) - [@mattaustin](https://twitter.com/mattaustin)
6. [Stored XSS at Parse](https://dr4cun0.com/blog/stored-xss-at-parse/) - [Dhaval](https://twitter.com/17haval) - No URL validation, Thus allowing `javascript:alert(1)` in URL parameter leading to XSS
7. [XSS in OAuth flow of Paypal](https://dr4cun0.com/blog/xss_in_oauth_flow_of_paypal-2/) - [Dhaval](https://twitter.com/17haval)
8. [Reflected XSS through AngularJS sandbox bypass...McDonald](https://finnwea.com/blog/stealing-passwords-from-mcdonalds-users) - [@finnwea](https://twitter.com/finnwea)
9. [Coming across an XSS vulnerability at Google sites is wrong I expected](http://nootropic.me/blog/en/blog/2016/09/20/%E3%82%84%E3%81%AF%E3%82%8A%E3%83%8D%E3%83%83%E3%83%88%E3%82%B5%E3%83%BC%E3%83%95%E3%82%A3%E3%83%B3%E3%82%92%E3%81%97%E3%81%A6%E3%81%84%E3%81%9F%E3%82%89%E3%81%9F%E3%81%BE%E3%81%9F%E3%81%BEgoogle/) - [ikuta_T](#)
10. [Hacking Google for fun and profit](https://introvertmac.wordpress.com/2016/07/30/hacking-google-for-fun-and-profit/#more-327) - [Manish Bhattacharya](https://twitter.com/UMeNMactech)
11. [Unpatched (0day) jQuery Mobile XSS](http://sirdarckcat.blogspot.in/2017/02/unpatched-0day-jquery-mobile-xss.html) - [EDUARDO VELA](https://twitter.com/sirdarckcat)
12. [Reflected XSS in Etsy](http://hmgmakarovich.blogspot.in/2017_01_01_archive.html) - [Harry M Gertos](http://hmgmakarovich.blogspot.in)
13. [Sleeping stored Google XSS Awakens a $5000 Bounty](https://blog.it-securityguard.com/bugbounty-sleeping-stored-google-xss-awakens-a-5000-bounty/) - [Patrik Fehrenbach ](https://twitter.com/ITSecurityguard)
14. [admin.google.com Reflected Cross-Site Scripting (XSS)](https://buer.haus/2015/01/21/admin-google-com-reflected-cross-site-scripting-xss/) - [Brett Buerhaus](https://twitter.com/bbuerhaus)
15. [Stored XSS at exchange.onavo.com](https://dr4cun0.com/blog/stored-xss-at-exchange-onavo-com/) - [Dhaval](https://twitter.com/17haval)
16. [Airbnb – When Bypassing JSON Encoding, XSS Filter, WAF](https://buer.haus/2017/03/08/airbnb-when-bypassing-json-encoding-xss-filter-waf-csp-and-auditor-turns-into-eight-vulnerabilities/) - [Brett Buerhaus](https://twitter.com/bbuerhaus)
17. [How I found a $5,000 Google Maps XSS](https://medium.com/@marin_m/how-i-found-a-5-000-google-maps-xss-by-fiddling-with-protobuf-963ee0d9caff) - [Marin Moulinier](#)

###### Cross Origin Resource Sharing Exploitation

1. [Think Outside the Scope: Advanced CORS Exploitation Techniques](https://medium.com/@sandh0t/think-outside-the-scope-advanced-cors-exploitation-techniques-dad019c68397) - [Sandh0t](#)

###### Cross Site Request Frogery - CSRF

1. [Messenger.com Site-Wide CSRF](https://whitton.io/articles/messenger-site-wide-csrf/) - [@fin1te](https://twitter.com/fin1te)
2. [How I bypassed Facebook CSRF once again!](http://blog.darabi.me/2016/05/how-i-bypassed-facebook-csrf-in-2016.html) - [Pouya Darabi](https://twitter.com/Pouyadarabi)

###### Server Side Request Frogery - SSRF

1. [SSRF at Facebook Update Subscription Menu](https://dr4cun0.com/blog/ssrf-at-update-subscription-menu/) - [Dhaval](https://twitter.com/17haval)
2. [Ok Google, Give Me All Your Internal DNS Information](https://www.rcesecurity.com/2017/03/ok-google-give-me-all-your-internal-dns-information/) - [Julien Ahrens
](https://twitter.com/mrtuxracer)
3. [How anyone could have used Uber to ride for free! ](http://www.anandpraka.sh/2017/03/how-anyone-could-have-used-uber-to-ride.html) - 

###### Application/Business Logic

1. [Facebook Simple Technical Bug worth 7500$](http://ashishpadelkar.com/index.php/2015/09/23/facebook-simple-technical-bug-worth-7500/) - [Ashish Padelkar](https://twitter.com/ashish_padelkar)
2. [How I Could Steal Money from Instagram, Google and Microsoft](https://www.arneswinnen.net/2016/07/how-i-could-steal-money-from-instagram-google-and-microsoft/) - [Arne Swinnen](https://twitter.com/arneswinnen)

###### SQL Injection - SQLi

1. [Popping a shell on the Oculus developer portal](https://bitquark.co.uk/blog/2014/08/31/popping_a_shell_on_the_oculus_developer_portal) - [Bitquark](https://twitter.com/Bitquark)
2. [SQLi + XXE + File path traversal Deutsche Telekom](https://www.ibrahim-elsayed.com/?p=150) - [Ibrahim M. El-Sayed](https://twitter.com/ibrahim_mosaad)
3. [GitHub Enterprise SQL Injection](http://blog.orange.tw/2017/01/bug-bounty-github-enterprise-sql-injection.html) - [Orange Tsai](#)

###### InDirect Object Reference - IDOR

1. [Facebook Vulnerability - Delete Any Video on Facebook](http://danmelamed.blogspot.in/2017/01/facebook-vulnerability-delete-any-video.html) - [Dan Melamed](https://twitter.com/danmelamed)
2. [Confirming new email/mobile number bug in Facebook](https://youtu.be/4euBQCMxlE8) - [Lokesh Kumar](#)
3. [How I hacked 62.5 million Zomato Users](http://www.anandpraka.sh/2015/06/how-i-hacked-zomatocom-to-see-data-of.html) - [Anand Prakash](https://twitter.com/sehacure) - [Anand Prakash](https://twitter.com/sehacure)

###### Code Execution

1. [Facebook’s ImageTragick Story](http://4lemon.ru/2017-01-17_facebook_imagetragick_remote_code_execution.html) - [@4lemon](https://twitter.com/4lemon)
2. [WD My Cloud Mirror 2.11.153 RCE and Authentication Bypass](https://security.szurek.pl/wd-my-cloud-mirror-211153-rce-and-authentication-bypass.html) - [Kacper Szurek](https://twitter.com/kacperszurek)
3. [0day writeup: XXE in uber.com](https://httpsonly.blogspot.in/2017/01/0day-writeup-xxe-in-ubercom.html) - [Vladimir Ivanov](https://twitter.com/httpsonly)
4. [Command injection which got me "6000$" from #Google](http://www.pranav-venkat.com/2016/03/command-injection-which-got-me-6000.html) - [S Venkatesh](http://www.pranav-venkat.com)
5. [Airbnb – Ruby on Rails String Interpolation led to Remote Code Execution](http://buer.haus/2017/03/13/airbnb-ruby-on-rails-string-interpolation-led-to-remote-code-execution/) - [Ben Sadeghipour Brett Buerhaus](#)
6.[GitHub Enterprise Remote Code Execution](http://exablue.de/blog/2017-03-15-github-enterprise-remote-code-execution.html) - [Markus Fenske](#)
7. [Escaping from Restricted Shell and Gaining Root Access](https://pentest.blog/unexpected-journey-4-escaping-from-restricted-shell-and-gaining-root-access-to-solarwinds-log-event-manager-siem-product/) - [Mehmet Ince](#)
8. [GitHub Enterprise Remote Code Execution](https://www.exablue.de/blog/2017-03-15-github-enterprise-remote-code-execution.html)

###### Reverse Engineering

1. [Unfolding obfuscated code with Reven (part 1)](http://blog.tetrane.com/2016/11/reversing-f4b-challenge-part1.html)
2. [Unfolding obfuscated code with Reven (part 2)](http://blog.tetrane.com/2016/11/reversing-f4b-challenge-part2.html)
3. [Three roads lead to Rome](http://blogs.360.cn/360safe/2016/11/29/three-roads-lead-to-rome-2/) - [Luke Viruswalker](#)

###### DNS Related

1. [Hijacking Broken Nameservers to Compromise Your Target](https://thehackerblog.com/respect-my-authority-hijacking-broken-nameservers-to-compromise-your-target/) - [@IAmMandatory](https://twitter.com/IAmMandatory)
2. [That (.) Which Made The Difference](https://dr4cun0.com/blog/that-which-made-the-difference/) - [Dhaval](https://twitter.com/17haval)
3. [Domain Fronting Via Cloudfront Alternate Domains](https://www.mdsec.co.uk/2017/02/domain-fronting-via-cloudfront-alternate-domains/) - [Vincent Yiu](https://twitter.com/vysecurity)

###### Brute-force

1. [How I could have hacked all Facebook accounts](http://www.anandpraka.sh/2016/03/how-i-could-have-hacked-your-facebook.html) - [Anand Prakash](https://twitter.com/sehacure)

###### Subdomain Takeover
1. [Hijacking tons of Instapage expired users Domains & Subdomains](http://www.geekboy.ninja/blog/tag/hackerone-subdomain-takeover) - [@emgeekboy](https://twitter.com/emgeekboy)
2. [The story of EV-SSL, AWS and trailing dot domains](https://labs.detectify.com/2016/10/05/the-story-of-ev-ssl-aws-and-trailing-dot-domains/) - [Detectify](https://twitter.com/detectify)

###### Open URL Redirection

1. [How I discovered a 1000$ open redirect in Facebook](http://yassineaboukir.com/blog/how-i-discovered-a-1000-open-redirect-in-facebook/) - [Yassine Aboukir](https://twitter.com/Yassineaboukir)
2. [Facebook Whitehat Vulnerability for 2013: Open Redirection in Facebook Mobile](https://prakharprasad.com/facebook-whitehat-vulnerability-for-2013-open-redirection-in-facebook-mobile/) - [Prakhar Prasad](https://twitter.com/prakharprasad)
3. [Dropbox Team Website Open Redirection](https://prakharprasad.com/dropbox-team-website-open-redirection/) - [Prakhar Prasad](https://twitter.com/prakharprasad)
4. [Bypassing SoundCloud’s protection for open redirections](https://strukt93.wordpress.com/2017/03/09/bypassing-soundclouds-protection-for-open-redirections/) - [strukt93](#)

###### XML Attacks

1. [eXtensible Markup Language Attacks](https://raviramesh.info/xml-attacks.html) - [Ravi Paghdal](https://twitter.com/_raviramesh)

###### HTTP Request Smuggling Desync Attack

1. [HTTP Request Smuggling Desync Attack](https://github.com/nachiketrathod/HTTP.Request.Smuggling.Desync.Attack)

###### Research Papers

1. [The Complete Guide to CORS (In)Security](https://www.bedefended.com/papers/cors-security-guide) - [Davide Danelon](https://twitter.com/@TwiceDi)

###### Miscellaneous

1. [Combining host header injection and lax host parsing serving malicious data](https://labs.detectify.com/2016/10/24/combining-host-header-injection-and-lax-host-parsing-serving-malicious-data/) - [Detectify](https://twitter.com/detectify)
2. [Compromising Apache Tomcat via JMX access](https://www.nccgroup.trust/uk/about-us/newsroom-and-events/blogs/2017/february/compromising-apache-tomcat-via-jmx-access/) - [NCC Group UK](#)
3. [Facebook's Bug - Unauthorized access to credit/prepaid card details](https://pranavhivarekar.in/2017/02/11/facebooks-bug-unauthorized-access-to-credit-card-details-limited-of-any-user/) - [Pranav Hivarekar](https://twitter.com/HivarekarPranav)
4. [Constructing an XSS vector, using no letters](https://inventropy.us/blog/constructing-an-xss-vector-using-no-letters) - [Charles Neill](https://twitter.com/ccneill)
5. [Order Facebook Friends by Facebook Recruiting Technical Coefficient](http://philippeharewood.com/order-facebook-friends-by-facebook-recruiting-technical-coefficient/) - [Philippe Harewood](https://twitter.com/phwd)
6. [Web Cache Deception Attack](http://omergil.blogspot.in/2017/02/web-cache-deception-attack.html) - [Omer Gil](https://twitter.com/omer_gil)
7. [Hacking Slack using postMessage and WebSocket](https://labs.detectify.com/2017/02/28/hacking-slack-using-postmessage-and-websocket-reconnect-to-steal-your-precious-token/) - [Frans Rosén](https://twitter.com/fransrosen)
8. [Stealing Messenger.com Login Nonces](https://stephensclafani.com/2017/03/21/stealing-messenger-com-login-nonces/) - [
Stephen Sclafani](https://twitter.com/Stephen)
9. [Escaping a Python sandbox with a memory corruption bug](https://medium.com/@gabecpike/python-sandbox-escape-via-a-memory-corruption-bug-19dde4d5fea5) - [Gabe Pike](#)
10. [Uploading web.config for Fun and Profit 2](https://soroush.secproject.com/blog/2019/08/uploading-web-config-for-fun-and-profit-2/) - [Soroush Dalili](https://twitter.com/irsdl)

###### Extras

1. [Everything you need to know about HTTP security headers](https://blog.appcanary.com/2017/http-security-headers.html)
2. [Helmet JS](https://helmetjs.github.io/docs/)
3. [GitHub's post-CSP journey](https://githubengineering.com/githubs-post-csp-journey/) - [Patrick Toomey](https://twitter.com/patricktoomey)
4. [CORS — a guided tour](https://medium.com/statuscode/cors-a-guided-tour-4e72230a8739#.bqddn2c22) - [Martin Splitt](#)
5. [Client Side Encryption Bypass](https://bhattsameer.github.io/2021/01/01/client-side-encryption-bypass-part-1.html) - [Sameer Bhatt](https://twitter.com/sameer_bhatt5)

#### Credits

###### Categories 
- [LtR101: Web Application Testing Methodologies](https://blog.zsec.uk/ltr101-methodologies/) - [Andy](https://twitter.com/ZephrFish)

## Stargazers over time

[![Stargazers over time](https://starchart.cc/dhaval17/awsome-security-write-ups-and-POCs.svg)](https://starchart.cc/dhaval17/awsome-security-write-ups-and-POCs)
