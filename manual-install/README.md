This folder contains regex-based blocklists. These need to be manually copied and pasted into the regex blacklist field in the pihole dashboard (or somewhere else if you prefer). The dashboard registeres space-separated blocks as different blocklists, so it's possible to copy-paste multiple at once 

# global-blocklist.regex.txt

Contains questionable websites that use subdomains actively.

# pridefall-blocklist.regex.txt

Contains all websites I've been able to find that have been (any of):

* Warned about (on twitter or similar)
* Shows up in Google searches for "ip logger" or "ip logger service", that also appears to be an IP logger
* Shows up in IP logging tutorials or similar

... as well as URL shorteners. It's important to note that the ones listed here are only the ones I know about. There may be more. There's also some extremely aggressive blocking, which is why there's an associated whitelist for domains I noticed breaks entirely. This notably includes wikipedia, because wik**ip**edia. The `.*ip.*` regex is extremely aggressive, and will result in false positives. If something breaks as a result, check the logs and whitelist the website.

This list may turn into a generalized IP logging blocklist when pridefall ends.

In the meanwhile, happy pride, and fuck pridefall! 
