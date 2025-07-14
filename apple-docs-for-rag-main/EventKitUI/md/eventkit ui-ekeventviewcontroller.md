

- EventKit UI
-  EKEventViewController 

Class

# EKEventViewController

A view controller for displaying existing calendar and reminder events, and for optionally editing those events.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class EKEventViewController
```

## Overview

The event view controller’s primary purpose is to present to the user a modal display containing the details of a calendar event. The view controller lets you set whether users may edit an event and, if the event is an invitation and the organizer is not the user, you can decide whether to show a preview of the event.

The event view controller includes delegates used to receive a notification when closing the view controller. The delegate must conform to the EKEventViewDelegate protocol.

## Topics

### Dismissing the Event Interface

var delegate: (any EKEventViewDelegate)?

The event view controller’s delegate.

protocol EKEventViewDelegate

Delegates used to display details for calendar events.

### Getting and Setting the Event

var event: EKEvent!

The event this view controller displays to the user.

### Displaying and Editing Event Previews

var allowsCalendarPreview: Bool

A Boolean that determines whether the user can preview the event in a calendar day.

var allowsEditing: Bool

A Boolean that determines whether the user may edit the event.

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

