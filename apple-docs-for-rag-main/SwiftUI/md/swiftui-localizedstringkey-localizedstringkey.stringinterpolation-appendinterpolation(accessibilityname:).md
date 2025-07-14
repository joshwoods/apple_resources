

- SwiftUI
- LocalizedStringKey
- LocalizedStringKey.StringInterpolation
-  appendInterpolation(accessibilityName:) 

Instance Method

# appendInterpolation(accessibilityName:)

Appends a localized description of a color for accessibility to a string interpolation.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
mutating func appendInterpolation(accessibilityName color: Color)
```

## Parameters 

`color`  

The color being described.

## Discussion

Don’t call this method directly; it’s used by the compiler when interpreting string interpolations.

