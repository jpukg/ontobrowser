# Introduction




A summary of the security review is provided in the sections below.

# Code Review

* Cross-Site Scripting (XSS)
* Cross-Site Request Forging (XSRF or CSRF)
* JSON and JSONP vulnerabilities



# Cross-Site Scripting (XSS)









 



* createChildTerm





Only one field (Term URL) was identified as a potentially security risk - using the javascript URL protocol (supported by all modern day graphical browsers) an attacker could inject arbitrary JavaScript code that would be run whenever any user clicked on the subsequent hyperlink (created from the Term URL user input). 


# Curator Password Protection ( installation)
