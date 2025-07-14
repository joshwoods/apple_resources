

- UIKit
-  UIUserInterfaceIdiom 

Enumeration

# UIUserInterfaceIdiom

Constants that indicate the interface type for the device or an object that has a trait environment, such as a view and view controller.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
enum UIUserInterfaceIdiom
```

## Topics

### Idioms

case unspecified

An unspecified idiom.

case phone

An interface designed for iPhone and iPod touch.

case pad

An interface designed for iPad.

case tv

An interface designed for tvOS and Apple TV.

case carPlay

An interface designed for an in-car experience.

case mac

An interface designed for the Mac.

case vision

An interface designed for visionOS and Apple Vision Pro.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Getting the current idiom

func UI_USER_INTERFACE_IDIOM() -> UIUserInterfaceIdiom

Returns the interface idiom supported by the current device (recommended for apps that run in versions of iOS earlier than 3.2).

Deprecated

