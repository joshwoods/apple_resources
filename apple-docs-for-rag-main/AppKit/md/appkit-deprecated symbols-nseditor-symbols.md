

- AppKit
- Deprecated Symbols
-  NSEditor 

# NSEditor

A set of methods that controllers and UI elements can implement to manage editing.

## Overview

The NSEditor informal protocol provides a means for requesting that the receiver commit or discard any pending edits.

These methods are typically invoked on user interface elements by a controller. They can also be sent to a controller in response to a user’s attempt to save a document or quit an application.

NSController provides an implementation of this protocol, as do the AppKit user interface elements that support binding.

Important

In macOS 10.7 or later, if you have enabled autosaving in your application, and your application has custom objects that implement or override the NSEditor protocol, you must also implement commitEditingWithoutPresentingError() in those objects.

## See Also

### Protocols

NSAccessibility

A legacy, informal protocol that Apple doesn’t recommend for active use.

protocol NSEditorRegistration

A set of methods that controllers can implement to enable an editor view to inform the controller when it has uncommitted changes.

protocol NSInputServiceProvider

protocol NSInputServerMouseTracker

protocol NSDrawerDelegate

A set of methods that drawer delegates implement to open, close, and resize the drawer.

Deprecated

