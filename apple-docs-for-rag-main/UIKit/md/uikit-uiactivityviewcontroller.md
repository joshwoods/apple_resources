

- UIKit
-  UIActivityViewController 

Class

# UIActivityViewController

A view controller that you use to offer standard services from your app.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class UIActivityViewController
```

## Mentioned in 

Collaborating and sharing copies of your data

## Overview

The system provides several standard services, such as copying items to the pasteboard, posting content to social media sites, sending items via email or SMS, and more. Apps can also define custom services.

Your app is responsible for configuring, presenting, and dismissing this view controller. Configuration for the view controller involves specifying the data objects on which the view controller should act. (You can also specify the list of custom services your app supports.) When presenting the view controller, you must do so using the appropriate means for the current device. On iPad, you must present the view controller in a popover. On iPhone and iPod touch, you must present it modally.

## Topics

### Initializing the activity view controller

init(activityItems: [Any], applicationActivities: [UIActivity]?)

Initializes a new activity view controller object that acts on the specified data.

convenience init(activityItemsConfiguration: any UIActivityItemsConfigurationReading)

Initializes a new activity view controller object that acts on the specified configuration.

class UIActivityItemsConfiguration

A configuration that allows a responder to export data through a variety of interactions.

protocol UIActivityItemsConfigurationReading

A set of methods adopted by an object so that the object can act as an activity items configuration.

### Accessing the completion handler

var completionWithItemsHandler: UIActivityViewController.CompletionWithItemsHandler?

The completion handler to execute after the activity view controller is dismissed.

typealias CompletionWithItemsHandler

A completion handler to execute after the activity view controller is dismissed.

### Excluding specific activity types

var excludedActivityTypes: [UIActivity.ActivityType]?

The list of services that should not be displayed.

### Excluding specific sections

var excludedActivitySectionTypes: UIActivitySectionTypes

struct UIActivitySectionTypes

### Elevating a prominent activity

var allowsProminentActivity: Bool

A Boolean value the system uses to elevate a system activity to make it more prominent.

### Deprecated

var completionHandler: UIActivityViewController.CompletionHandler?

The completion handler to execute after the activity view controller is dismissed.

Deprecated

typealias CompletionHandler

A completion handler to execute after the activity view controller is dismissed.

Deprecated

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

### Services

class UIActivity

An abstract class that you subclass to implement app-specific services.

protocol UIActivityItemSource

A set of methods that an activity view controller uses to retrieve the data items to act on.

class UIActivityItemProvider

A proxy for data that passes to an activity view controller.

