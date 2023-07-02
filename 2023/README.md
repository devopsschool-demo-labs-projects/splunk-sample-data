# What is in the tutorial data?
The tutorial data file is updated daily and contains events that are timestamped for the previous seven days. The tutorial data contains several types of information about the fictitious online store Buttercup Games. Buttercup, for those of you that don't know, is a pony and is the Splunk mascot.

The information includes access.log files, secure.log files, and vendor_sales.log files from mail servers and web accounts.

# access.log file data
The raw data in the access.log file is difficult to read and analyze when you have hundreds, if not thousands, of lines of data. Each day, every day. That is where the Splunk platform comes in.

```
175.44.24.82 - - [22/Feb/2021:18:44:40] "POST /product.screen?productId=WC-SH-A01&JSESSIONID=SD7SL9FF5ADFF5066 HTTP 1.1" 200 3067 "http://www.buttercupgames.com/product.screen?productId=WC-SH-A01" "Mozilla/5.0 (compatible; MSIE 9.0; Windows NT 6.1; WOW64; Trident/5.0; BOIE9;ENUS)" 307
142.233.200.21 - - [22/Feb/2021:19:20:13] "GET show.do?productId=SF-BVS-01&JSESSIONID=SD6SL8FF4ADFF5218 HTTP 1.1" 404 1329 "http://www.buttercupgames.com/cart.do?action=purchase&itemId=EST-13" "Mozilla/5.0 (compatible; Googlebot/2.1; +http://www.google.com/bot.html)" 674
```

# secure.log file data

The raw data in the secure.log file looks like this:
```
Thu Mar 22 2021 00:15:06 mailsv1 sshd[60445]: pam_unix(sshd:session): session opened for user mdubios by (uid=0)
Thu Mar 22 2021 00:15:06 mailsv1 sshd[3759]: Failed password for djohnson from 194.8.74.23 port 3769 ssh2
Thu Mar 22 2021 00:15:08 mailsv1 sshd[5276]: Failed password for invalid user appserver from 194.8.74.23 port 3351
```
# vendor_sales.log file data
The raw data in the vendor_sales.log file looks like this:
```
[13/Apr/2021:18:23:07] VendorID=5037 Code=C AcctID=5317605039838520
[13/Apr/2021:18:23:22] VendorID=9108 Code=A AcctID=2194850084423218
[13/Apr/2021:18:23:49] VendorID=1285 Code=F AcctID=8560077531775179
[13/Apr/2021:18:23:59] VendorID=1153 Code=D AcctID=4433276107716482
```
