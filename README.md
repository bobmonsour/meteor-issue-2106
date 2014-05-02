## Reproduction for Meteor issue 2106

- https://github.com/meteor/meteor/issues/2106

1. Clone the repository

1. Open the javascript console

2. Start the app in Meteor 0.8.1 or 0.8.1.1

3. Observe the app display squares in place of the proper Font Awesome icons

4. Note the console display of the following:

  "Resource interpreted as Font but transferred with MIME type text/html..."

  For 3 of the 5 font files in the client/fonts directory:
    - fontawesome-webfont.woff?v=4.0.3 
    - fontawesome-webfont.ttf?v=4.0.3 
    - fontawesome-webfont.svg?v=4.0.3

  The other two files generate no such message:
    - fontawesome-webfont.eot
    - FontAwesome.otf

  Expected: to see the heart icon display

  Actual: square is displayed
