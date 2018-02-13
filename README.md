# Denial of service Attack on Chrome (memory leak vulnerability)

Steps to reproduce the attack : 

1. Send the "Page.html" file to a user( or host the file somewhere and send the link to the user )
2. The user opens the "Page.html" file on Chrome.


Brief Description of what will happen :

-on PC : 
1.the script will start allocate memory at a rate of 10MB/s which reduces the performance of the computer in few minutes.
2.if the user is in an other tab no alert is shown
  else a "page unresponsive" message is shown with a "wait" button

-on Android :
1.the script will start allocate memory at a rate of 10MB/s which reduces the performance of the smartphone and causes the app to freeze.

Remarque : 
this attack was reported to google , it got a "WontFix" statut.
https://chromium.googlesource.com/chromium/src/+/master/docs/security/faq.md#Are-denial-of-service-issues-considered-security-bugs
