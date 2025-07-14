

- WatchKit
- WKInterfacePaymentButton
-  init(target:action:) 

Initializer

# init(target:action:)

Creates a payment button for use in SwiftUI.

watchOS 6.0+

``` source
init(
    target: Any?,
    action: Selector
)
```

## Parameters 

`target`  

The object whose action method is called.

`action`  

A selector identifying the action method called when the user taps the button.

## Discussion

When the user taps the button, the system calls the `action` method on the `target`.

Use this initializer to create an instance that you can wrap in a WKInterfaceObjectRepresentable view. If you aren’t using SwiftUI, create the control by dragging it from the Object library to your storyboard instead.

