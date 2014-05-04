# Dashkiosk

Dashkiosk is a solution to manage dashboards on multiple screens. It
comes as four components:

 1. A _receiver_ runs in a browser attached to each screen and will
    display the requested dashboards. The receiver is quite dumb, it
    contacts the server and wait for it to tell which URL to display.

 2. A _server_ which will manage the screens by sending them what they
    should display. An administration interface allows the user to
    manage those screens individually or in a group.
    
 3. An _Android app_ that will run the receiver. This is mainly a
    fullscreen webview.

 4. A _Chromecast custom receiver_ which will run the regular receiver
    if you want to display dashboards using Google Chromecast devices.

The full documentation is available on [ReadTheDocs][].

[ReadTheDocs]: http://dashkiosk.readthedocs.org

Here is a demonstration video:

<iframe frameborder="0" width="480" height="270"
        src="//www.dailymotion.com/embed/video/x1sy4x7"
        allowfullscreen></iframe>

# Development

To run the server for development:

    $ grunt serve
