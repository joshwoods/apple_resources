

- SwiftUI
- BorderedButtonStyle
-  makeBody(configuration:) 

Instance Method

# makeBody(configuration:)

Creates a view that represents the body of a button.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 7.0+

``` source
@MainActor @preconcurrency
func makeBody(configuration: BorderedButtonStyle.Configuration) -> some View
```

## Parameters 

`configuration`  

The properties of the button.

## Discussion

The system calls this method for each Button instance in a view hierarchy where this style is the current button style.

