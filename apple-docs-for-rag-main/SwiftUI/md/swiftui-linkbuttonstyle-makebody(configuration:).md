

- SwiftUI
- LinkButtonStyle
-  makeBody(configuration:) 

Instance Method

# makeBody(configuration:)

Creates a view that represents the body of a button.

macOS 10.15+

``` source
@MainActor @preconcurrency
func makeBody(configuration: LinkButtonStyle.Configuration) -> some View
```

## Parameters 

`configuration`  

The properties of the button.

## Discussion

The system calls this method for each Button instance in a view hierarchy where this style is the current button style.

