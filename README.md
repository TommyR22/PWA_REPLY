## Usage
Download and use a web server like: https://chrome.google.com/webstore/detail/web-server-for-chrome/ofhbbkphhbklhfoeikjpcbhemlocgigb

# TODO

-   Manifest
    <!--<link rel="manifest" href="manifest.json">-->

    <!--Add to home screen for Safari on iOS-->
    <!--<meta name="apple-mobile-web-app-capable" content="yes">-->
    <!--<meta name="apple-mobile-web-app-status-bar-style" content="black">-->
    <!--<meta name="apple-mobile-web-app-title" content="Weather Reply">-->
    <!--<link rel="apple-touch-icon" href="images/icons/icon-152x152.png">-->
    <!--<meta name="msapplication-TileImage" content="images/icons/icon-144x144.png">-->
    <!--<meta name="msapplication-TileColor" content="#2F3BA2">-->
    
-   Cache localStorage
    add : app.saveSelectedCities(); in document.getElementById('butAddCity')
    add:  app.saveSelectedCities(); in startup code.

    app.saveSelectedCities = function () {
            var selectedCities = JSON.stringify(app.selectedCities);
            localStorage.selectedCities = selectedCities;
    };

-   Service Worker

    - change pattern SW

    - push notification
        https://developers.google.com/web/ilt/pwa/introduction-to-push-notifications

        add in manifest.json: "gcm_sender_id": "44474987793"

        curl "ENDPOINT_URL" --request POST --header "TTL: 60" --header "Content-Length: 0" --header "Authorization: key=SERVER_KEY"

        Chrome bug: https://github.com/GoogleChromeLabs/web-push-codelab/issues/49


-   Change localStorage with IndexedDb

-   Google Lighthouse




