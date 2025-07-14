

- Shared With You
-  SWRemoveParticipantAlertController 

Class

# SWRemoveParticipantAlertController

The view controller for the remove-participant alert.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
class SWRemoveParticipantAlertController
```

## Topics

### Creating the alert controller

convenience init(participant: SWPerson, highlight: SWCollaborationHighlight)

Creates and initializes the alert controller.

## Relationships

### Inherits From

- UIViewController

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSExtensionRequestHandling
- NSObjectProtocol
- NSTouchBarProvider
- Sendable
- UIActivityItemsConfigurationProviding
- UIAppearanceContainer
- UIContentContainer
- UIFocusEnvironment
- UIPasteConfigurationSupporting
- UIResponderStandardEditActions
- UIStateRestoring
- UITraitChangeObservable
- UITraitEnvironment
- UIUserActivityRestoring

## See Also

### Requesting participant removal

class func show(withParticipant: SWPerson, highlight: SWCollaborationHighlight, in: NSWindow?)

