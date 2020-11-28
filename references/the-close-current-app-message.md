# The "close current app" message

Broadcast the "close current app" message to remove the "[active app](variables-and-lists/active-app.md)"'s value from the "[opened apps](variables-and-lists/opened-apps.md)" list and it will automatically set another one as the "[active app](variables-and-lists/active-app.md)"'s value.

* If there's a next app in ["opened apps](variables-and-lists/opened-apps.md)" list, it will be set as "[active app](variables-and-lists/active-app.md)".
* Else, if there's a previous app in "[opened apps](variables-and-lists/opened-apps.md)" list, it will be set.
* Else, it will set "[active app](variables-and-lists/active-app.md)" to "none".

