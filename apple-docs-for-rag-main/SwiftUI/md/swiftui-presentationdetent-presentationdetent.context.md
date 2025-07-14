

- SwiftUI
- PresentationDetent
-  PresentationDetent.Context 

Structure

# PresentationDetent.Context

Information that you use to calculate the presentation’s height.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
@dynamicMemberLookup
struct Context
```

## Topics

### Getting the height

var maxDetentValue: CGFloat

The height that the presentation appears in.

### Supporting types

subscript&lt;T>(dynamicMember _: KeyPath&lt;EnvironmentValues, T>) -> T

Returns the value specified by the keyPath from the environment.

## See Also

### Creating custom detents

static func custom&lt;D>(D.Type) -> PresentationDetent

A custom detent with a calculated height.

static func fraction(CGFloat) -> PresentationDetent

A custom detent with the specified fractional height.

static func height(CGFloat) -> PresentationDetent

A custom detent with the specified height.

