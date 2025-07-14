

- UIKit
- UIActivityViewController
-  UIActivityViewController.CollaborationModeRestriction 

Class

# UIActivityViewController.CollaborationModeRestriction

An object that disables the sharing mode and optionally displays an alert.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+visionOS 2.0+

``` source
class CollaborationModeRestriction
```

## Mentioned in 

Collaborating and sharing copies of your data

## Topics

### Creating a disabled mode

init(disabledMode: UIActivityCollaborationMode)

Copies the provided disabled mode.

init(disabledMode: UIActivityCollaborationMode, alertTitle: String, alertMessage: String)

Creates a disabled mode that displays an alert when someone tries to select that mode.

init(disabledMode: UIActivityCollaborationMode, alertTitle: String, alertMessage: String, alertDismissButtonTitle: String)

Creates a disabled mode that displays an alert with a customized dismiss button.

init(disabledMode: UIActivityCollaborationMode, alertTitle: String, alertMessage: String, alertDismissButtonTitle: String, alertRecoverySuggestionButtonTitle: String, alertRecoverySuggestionButtonLaunch: URL)

Creates a disabled mode that displays an alert with a recovery suggestion.

### Accessing the disabled mode’s properties

var alertDismissButtonTitle: String?

A title for the alert’s dismiss button.

var alertMessage: String?

A message displayed by the alert

var alertRecoverySuggestionButtonLaunchURL: URL?

A launch URL that the system passes to your app when someone taps the recovery suggestion button.

var alertRecoverySuggestionButtonTitle: String?

A title for the alert’s recovery suggestion button.

var alertTitle: String?

A title for the alert that the system displays when someone selects the disabled mode.

var disabledMode: UIActivityCollaborationMode

The mode that is disabled.

func description() -> String

Returns a description of the disabled mode.

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

## See Also

### Restricting the sharing mode

enum UIActivityCollaborationMode

A value that defines how the system shares an item.

