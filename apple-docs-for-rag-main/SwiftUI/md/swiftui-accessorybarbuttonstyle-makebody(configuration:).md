

- SwiftUI
- AccessoryBarButtonStyle
-  makeBody(configuration:) 

Instance Method

# makeBody(configuration:)

Creates a view that represents the body of a button.

macOS 14.0+

``` source
@MainActor @preconcurrency
func makeBody(configuration: AccessoryBarButtonStyle.Configuration) -> some View
```

## Parameters 

`configuration`  

The properties of the button.

## Discussion

The system calls this method for each Button instance in a view hierarchy where this style is the current button style.

