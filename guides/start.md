# Getting started \(explanations version\)

### How does Feather Desktop works ?

For Feather Desktop, while its multitasking can seem complex, it's actually pretty simple.

The only thing that constitute its core is the "close app" method, which can be triggered by sending the ["close current app" message](../references/the-close-current-app-message.md).

This method relies on some variables and lists :

* [The `opened apps` list](../references/variables-and-lists/opened-apps.md), which hold the current opened apps' IDs.
* [The `active app` variable](../references/variables-and-lists/active-app.md), which holds the opened app that should be shown on screen as active app's ID.

An ID is simply a number that you will use to refer your app.

In the Feather Desktop original project, the IDs correspond to the costumes numbers for the app icons, in the sprite that manages the display of the taskbar apps.

### How can I use these to make a project off of Feather Desktop ?

The sprites that constitute your app can watch [the `active app` variable](../references/variables-and-lists/active-app.md)'s value, and if it's corresponding to their apps ID, you will likely make them show, otherwise, you will likely hide them.

You can also watch [the `opened apps` list](../references/variables-and-lists/opened-apps.md) with one or more sprite to show opened apps in a taskbar or another thing like this, or even making a "real" window system with multiple windows, using this list with [the `active app` variable](../references/variables-and-lists/active-app.md) to know what windows to show, and which of them should be at front.

