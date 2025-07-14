

- TVMLKit JS
-  App 

Class

# App

An object that provides access to—and a means to respond to—app life-cycle events.

tvOS 9.0+

``` source
interface App
```

## Overview

You cannot create an instance of the `App` class. An instance of this class is available in the global context as `App`.

## Topics

### Responding to App Life Cycle Events

onError

A callback function that is automatically called when an error is sent from the Apple TV.

onExit

A callback function that is automatically called when the app has been exited.

onLaunch

A callback function that is automatically called when the app has been launched.

onResume

A callback function that is automatically called when the app moves to the foreground.

onSuspend

A callback function that is automatically called when the app is sent to the background.

### Reloading the App

reload

Reloads the app.

### Instance Properties

onDocumentRequest

## See Also

### App Initialization

UserDefaults

An object that contains the app's default preferences.

NavigationDocument

A document stack that holds the individual TVML documents for a client-server app.

Responding to User Interaction

Update onscreen information by adding event listeners to your Apple TV app.

EventListenerObject

An object that communicates events and allows other objects to add themselves as listeners.

