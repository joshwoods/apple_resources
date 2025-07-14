

- SwiftUI
- PresentationDetent
-  custom(\_:) 

Type Method

# custom(\_:)

A custom detent with a calculated height.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
static func custom(_ type: D.Type) -> PresentationDetent where D : CustomPresentationDetent
```

## See Also

### Creating custom detents

static func fraction(CGFloat) -> PresentationDetent

A custom detent with the specified fractional height.

static func height(CGFloat) -> PresentationDetent

A custom detent with the specified height.

struct Context

Information that you use to calculate the presentation’s height.

