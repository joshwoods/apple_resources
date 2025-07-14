

- WatchKit
- WKInterfaceAuthorizationAppleIDButton
-  init(style:target:action:) 

Initializer

# init(style:target:action:)

Creates an authorization button for use in SwiftUI.

watchOS 6.1+

``` source
init(
    style: WKInterfaceAuthorizationAppleIDButton.Style,
    target: Any?,
    action: Selector
)
```

## Parameters 

`style`  

The button’s style. For a list of possible values, see WKInterfaceAuthorizationAppleIDButton.Style.

`target`  

The object whose action method is called.

`action`  

A selector identifying the action method called when the user taps the button.

## Discussion

When the user taps the button, the system calls the `action` method on the target.

Use this initializer to create an instance that you can wrap in a WKInterfaceObjectRepresentable view. If you aren’t using SwiftUI, create the control by dragging it from the Object library to your storyboard instead.

## See Also

### Initializing for SwiftUI

enum Style

Values that define an authorization button’s style.

init(target: Any?, action: Selector)

Creates an authorization button for use in SwiftUI.

Deprecated

