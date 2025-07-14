

- UIKit
- UIApplication
-  UIApplication.ExtensionPointIdentifier 

Structure

# UIApplication.ExtensionPointIdentifier

A structure that identifies types of extensions.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
struct ExtensionPointIdentifier
```

## Topics

### Constants

static let keyboard: UIApplication.ExtensionPointIdentifier

The identifier for custom keyboards.

### Initializers

init(rawValue: String)

Creates a new instance with the specified raw value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Disallowing specified app extension types

func application(UIApplication, shouldAllowExtensionPointIdentifier: UIApplication.ExtensionPointIdentifier) -> Bool

Asks the delegate to grant permission to use app extensions that are based on a specified extension point identifier.

static let keyboard: UIApplication.ExtensionPointIdentifier

The identifier for custom keyboards.

