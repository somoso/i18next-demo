i18next demo
=========

This is a demo for how to use the i18next library, after I spent an hour after work going mental trying to figure it out from the lack of clearly defined documentation at the time of writing.

contents
--------

* A barebones HTML file with a script in the body that shows i18n in action in the console window of your browser.

* i18next library *and* the i18next XHR backend - in order to fetch files from disk, you need a i18next backend - this was something that wasn't painfully clear to me when I was browsing the i18next documentation.

* Some demo translation files in "locales". You will see 'dev' and 'en' because while debugging i18next complained about their absence (it still produced what I wanted though, but that's because I purposely produced the right locales for me)

information
-----------

If you are to read localised json files from your server, you absolutely must need a backend - this cannot be stressed enough. Otherwise the i18next can only give localisations from a JSON array embedded in the i18n options parameter. Also, don't forget the callback in init returns two parameters - the right translation object and an error.