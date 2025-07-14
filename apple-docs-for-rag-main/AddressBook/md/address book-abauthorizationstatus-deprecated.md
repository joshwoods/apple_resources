

- Address Book
-  ABAuthorizationStatus Deprecated

Enumeration

# ABAuthorizationStatus

Different possible values for the authorization status of an app with respect to address book data.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
enum ABAuthorizationStatus
```

Deprecated

use CNAuthorizationStatus

## Topics

### Constants

case notDetermined

No authorization status could be determined.

case restricted

The app is not authorized to access address book data. The user cannot change this access, possibly due to restrictions such as parental controls.

case denied

The user explicitly denied access to address book data for this app.

case authorized

The app is authorized to access address book data.

### Initializers

init?(rawValue: CFIndex)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Deprecated

struct ABPersonImageFormat

Indicates an image format.

Deprecated

