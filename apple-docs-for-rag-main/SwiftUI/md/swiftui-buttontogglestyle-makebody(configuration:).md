

- SwiftUI
- ButtonToggleStyle
-  makeBody(configuration:) 

Instance Method

# makeBody(configuration:)

Creates a view that represents the body of a toggle button.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+visionOS 1.0+watchOS 9.0+

``` source
@MainActor @preconcurrency
func makeBody(configuration: ButtonToggleStyle.Configuration) -> some View
```

## Parameters 

`configuration`  

The properties of the toggle, including a label and a binding to the toggle’s state.

## Return Value

A view that acts as a button that controls a Boolean state.

## Discussion

SwiftUI implements this required method of the ToggleStyle protocol to define the behavior and appearance of the button toggle style. Don’t call this method directly; the system calls this method for each Toggle instance in a view hierarchy that’s styled as a button.

