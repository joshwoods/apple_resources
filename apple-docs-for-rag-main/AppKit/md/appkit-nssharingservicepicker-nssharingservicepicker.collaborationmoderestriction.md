

- AppKit
- NSSharingServicePicker
-  NSSharingServicePicker.CollaborationModeRestriction 

Class

# NSSharingServicePicker.CollaborationModeRestriction

macOS 15.0+

``` source
class CollaborationModeRestriction
```

## Topics

### Initializers

init(disabledMode: NSSharingCollaborationMode)

init(disabledMode: NSSharingCollaborationMode, alertTitle: String, alertMessage: String)

init(disabledMode: NSSharingCollaborationMode, alertTitle: String, alertMessage: String, alertDismissButtonTitle: String)

init(disabledMode: NSSharingCollaborationMode, alertTitle: String, alertMessage: String, alertDismissButtonTitle: String, alertRecoverySuggestionButtonTitle: String, alertRecoverySuggestionButtonLaunch: URL)

### Instance Properties

var alertDismissButtonTitle: String?

The label on the alert button which will simply confirm that the alert was viewed and dismiss it Defaults to “OK”

var alertMessage: String?

The message of the alert if a reason for disabling is provided

var alertRecoverySuggestionButtonLaunchURL: URL?

The URL that is opened when the user selects the recovery suggestion, if any

var alertRecoverySuggestionButtonTitle: String?

The label on the recovery suggestion button if it is provided

var alertTitle: String?

The title of the alert if a reason for disabling is provided

var disabledMode: NSSharingCollaborationMode

The type of sharing which should be disabled

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- NSSecureCoding

