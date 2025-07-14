

- Group Activities
-  GroupActivitySharingController 

Class

# GroupActivitySharingController

An iOS view controller that displays the system interface for starting an activity, and optionally starts a FaceTime call for that activity.

GroupActivitiesUIKitiOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+visionOS 1.0+

``` source
@MainActor @objc
class GroupActivitySharingController
```

## Overview

A GroupActivitySharingController helps you start a SharePlay activity, even when a FaceTime call isn’t currently active. When presented, the view controller prompts the person to start the activity you provided. If no FaceTime call is active, the view controller also displays a people picker to let the person select the participants for the activity. When they choose to start the activity, the view controller automatically starts the FaceTime call as needed and joins your app to the activity.

If your app’s interface includes controls to start SharePlay activities, present this view controller in response to interactions with those controls. Initialize the GroupActivitySharingController object with the activity you want to start. After you present it, the view controller handles all further interactions. It manages the interface that appears onscreen and responds when someone chooses to start or cancel the activity. It starts the FaceTime call if one isn’t currently active. It also dismisses itself and returns control back to your app, updating its result property to let you know what happened.

## Topics

### Creating the group activity sharing controller

init&lt;ActivityType>(ActivityType) throws

Initializes the sharing controller with the specified activity and type information.

init&lt;ActivityType>(preparationHandler: () async throws -> ActivityType)

Initializes the SharePlay sharing controller with a closure that creates the activity object.

### Getting the result

var result: GroupActivitySharingResult

The result of a request to share a group activity.

enum GroupActivitySharingResult

The result of a request to share a group activity in iOS.

### Responding to view-related events

func viewDidLoad()

Notifies the view controller that the system added a view to a view hierarchy.

func viewWillAppear(Bool)

Notifies the view controller that the system is going to add a view to a view hierarchy.

### Instance Properties

var modalPresentationStyle: UIModalPresentationStyle

The presentation style for the view controller.

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

### Interface presentation

Presenting SharePlay activities from your app’s UI

Make it easy for people to start activities from your app’s UI, from the system share sheet, or using AirPlay over AirDrop.

class GroupActivitySharingController

A macOS view controller that displays the system interface for starting an activity, and optionally starts a FaceTime call for that activity.

