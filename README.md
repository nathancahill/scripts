# Scripts

## Google Voice Growl Notifier

Adds much needed Growl functionality to Google Voice. The Google Voice webpage never refreshes like Gmail does to get a (1) in the title. At the heart of the program is a perl script that polls Google Voice for new messages.
Since I haven't built a login system yet, it uses a cookies.txt file which contains the appropriate Google Voice cookie. It's controlled by a launch daeomon, so it starts on on boot.

### To install:

1. Copy com.nathancahill.gv_notifier.plist to /Library/LaunchDaemons/
2. Save the Google Voice cookies to cookies.txt in 'Google Voice Notifier'
3. Copy 'Google Voice Notifier' to /Library/Application Support/

### Exporting cookies:

For Firefox, install the Export Cookies addon. ![https://addons.mozilla.org/en-US/firefox/addon/cookie-exporter/?src=api](https://addons.mozilla.org/en-US/firefox/addon/cookie-exporter/?src=api])

For Chrome, install the cookies.txt export extension. ![https://chrome.google.com/webstore/detail/lopabhfecdfhgogdbojmaicoicjekelh](https://chrome.google.com/webstore/detail/lopabhfecdfhgogdbojmaicoicjekelh)

Safari is a bit trickier, there's a great little ruby script by Serious Orange to tackle the problem. ![http://seriousorange.com/2010/01/converting-safari-cookies-plist-to-cookies-txt/](http://seriousorange.com/2010/01/converting-safari-cookies-plist-to-cookies-txt/)
