# iOS-code-test

The future is a fantastic place where monetary systems have been replaced by
Bitcoin and humans have evolved to get all of their nutrients from burgers.

It is in this future that you have been recruited to VolcanoSolutions as a mobile developer. Your first task is to develop an app that allows your fellow
hungry coworkers to browse the burgers that are available at the universe's
most popular chain Coffee Port.

Coffee Port have an API available at http://coffeeport.herokuapp.com/

A list of burgers is available at http://coffeeport.herokuapp.com/burgers/ and
has the following structure:

    {
        "latency": 1, 
        "burgers": [
            {
                "vegetarian": true, 
                "name": "Seitan Burger", 
                "promoted": false, 
                "id": 1, 
                "image": "/static/burgers/seitan.jpg", 
                "bitcoin": 599, 
                "notes": "Made from seitan in the Cetus system, imported to
                Coffee Port by the Intergalactic Vegan Association."
            }
        ]
    }

Buying a burger is done by POSTing some JSON to the same address. The JSON is:

    {
        id: <burger id>,
        bitcoin: <integer value of the bitcoin price>
    }

The app should have a single horizontally scrollable promoted burger section
displaying the burger's name, price, mouth-watering image, vegetarian indicator
(a 'V' will suffice), and a button to buy.

The non-promoted burgers should be listed one-at-a-time beneath the promoted
burgers and have a small thumbnail, name, price, button, and vegetarian
indicator.

Because of the connection not being always stable everywhere even in the future, the app 
must cache the data for offline access although the buttons should be disabled
if there is no connection available.

When an order has been successfully made an alert should be congratulating the
user for their excellent choice!

If the user taps on a burger - but not the buy button - an alert should display
any extra notes associated.

# ADDENDUM

You are free to use any libraries you wish.

You are allowed to use obj-c, but here at Volcanos we try to use the newest technologies so the latest version of Swift is highly encouraged.

Try not to get too hungry while developing the app and accidentally eat your
phone.
