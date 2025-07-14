

- SwiftUI
- PlainButtonStyle
-  makeBody(configuration:) 

Instance Method

# makeBody(configuration:)

Creates a view that represents the body of a button.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@MainActor @preconcurrency
func makeBody(configuration: PlainButtonStyle.Configuration) -> some View
```

## Discussion

The system calls this method for each Button instance in a view hierarchy where this style is the current button style.

