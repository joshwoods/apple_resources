

- UIKit
- UIResponder
-  keyCommands 

Instance Property

# keyCommands

The key commands that trigger actions on this responder.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var keyCommands: [UIKeyCommand]? { get }
```

## Discussion

A responder object that supports hardware keyboard commands can redefine this property and use it to return an array of UIKeyCommand objects that it supports. Each key command object represents the keyboard sequence to recognize and the action method of the responder to call in response.

The key commands you return from this method are applied to the entire responder chain. When a key combination is pressed that matches a key command object, UIKit walks the responder chain looking for an object that implements the corresponding action method. It calls that method on the first object it finds and then stops processing the event.

