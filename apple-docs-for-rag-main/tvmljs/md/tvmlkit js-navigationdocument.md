

- TVMLKit JS
-  NavigationDocument 

Class

# NavigationDocument

A document stack that holds the individual TVML documents for a client-server app.

tvOS 9.0+

``` source
interface NavigationDocument
```

## Overview

You cannot create an instance of the `NavigationDocument` class. An instance of this class is available in the global context as `navigationDocument`.

## Topics

### Adding Documents to the Stack

insertBeforeDocument

Inserts a new document directly before a document currently on the stack.

pushDocument

Pushes the specified document onto the stack.

replaceDocument

Replaces a document on the stack with a new document.

### Overlaying Document

dismissModal

Dismisses the document displayed in modal view.

presentModal

Displays the passed document on top of the current document.

### Viewing the Stack

documents

The documents currently on the stack.

### Removing Documents from the Stack

clear

Removes all documents currently on the stack.

popDocument

Removes the top most document from the stack.

popToDocument

Removes all of the documents on the stack that are above the passed document.

popToRootDocument

Removes all documents from the stack except for the bottom-most document, which is the root document.

removeDocument

Removes the specified document from the stack.

## See Also

### App Initialization

App

An object that provides access to—and a means to respond to—app life-cycle events.

UserDefaults

An object that contains the app's default preferences.

Responding to User Interaction

Update onscreen information by adding event listeners to your Apple TV app.

EventListenerObject

An object that communicates events and allows other objects to add themselves as listeners.

