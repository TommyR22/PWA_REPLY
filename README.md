## Install
Download and use a web server like: [web-server-for-chrome](https://chrome.google.com/webstore/detail/web-server-for-chrome/ofhbbkphhbklhfoeikjpcbhemlocgigb)

or use python: `python -m SimpleHTTPServer` (Python 2.7) / `python -m http.server --cgi 8000` (Python 3.7)

#TODO

## Manifest
* create manifest.json and add it to project.
    * you can find icons in `images/icons` folder.
* link it to index.html
* test it with Chrome DevTool.
    
## Cache localStorage
* create a function to save `app.selectedCities` in localStorage.
* call this function in `butAddCity` eventListener.
* call this function in startup code.

## Service Worker
* create a service worker file
    * handle INSTALL, ACTIVATE and FETCH event.
    * In FETCH event, use a cache pattern.
* register it in app.js
* (OPTIONAL) change pattern ServiceWorker
* (OPTIONAL) push notification
    * follow this guide: https://developers.google.com/web/ilt/pwa/introduction-to-push-notifications
    * add in manifest.json: "gcm_sender_id": "ID_NUMBER"
    * curl "ENDPOINT_URL" --request POST --header "TTL: 60" --header "Content-Length: 0" --header "Authorization: key=SERVER_KEY"

Chrome bug: https://github.com/GoogleChromeLabs/web-push-codelab/issues/49


## IndexedDB
Change localStorage with IndexedDB

# Testing
* use Google Lighthouse




