

- SwiftUI
- CardButtonStyle
-  makeBody(configuration:) 

Instance Method

# makeBody(configuration:)

Creates a view that represents the body of a button.

tvOS 14.0+

``` source
@MainActor @preconcurrency
func makeBody(configuration: CardButtonStyle.Configuration) -> some View
```

## Parameters 

`configuration`  

The properties of the button.

## Discussion

The system calls this method for each Button instance in a view hierarchy in which CardButtonStyle is the current button style.

