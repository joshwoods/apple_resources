

- UIKit
- UIScene
-  UIScene.OpenExternalURLOptions 

Class

# UIScene.OpenExternalURLOptions

Options you specify when asking a scene to open a URL.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
class OpenExternalURLOptions
```

## Topics

### Specifying the link options

var universalLinksOnly: Bool

A Boolean value that indicates whether URLs must be universal links and have a configured app to open them.

### Measuring ad taps

var eventAttribution: UIEventAttribution?

An object you use to send tap event attribution data to the browser for Private Click Measurement.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### URL management

class UIOpenURLContext

A system-provided object that contains the information you need to open a single URL.

