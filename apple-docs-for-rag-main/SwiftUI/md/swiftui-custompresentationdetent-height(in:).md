

- SwiftUI
- CustomPresentationDetent
-  height(in:) 

Type Method

# height(in:)

Calculates and returns a height based on the context.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func height(in context: Self.Context) -> CGFloat?
```

**Required**

## Parameters 

`context`  

Information that can help to determine the height of the detent.

## Return Value

The height of the detent, or `nil` if the detent should be inactive based on the `contenxt` input.

## See Also

### Getting the height

typealias Context

Information that you can use to calculate the height of a custom detent.

