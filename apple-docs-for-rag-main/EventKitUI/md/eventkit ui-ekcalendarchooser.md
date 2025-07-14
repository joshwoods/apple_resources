

- EventKit UI
-  EKCalendarChooser 

Class

# EKCalendarChooser

A view controller for determining whether a user may select one or more calendars.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.0+visionOS 1.0+

``` source
@MainActor
class EKCalendarChooser
```

## Overview

Use the calendar chooser view controller to allow users to select one or more calendars when creating or editing a calendar event. The calendar chooser also lets you specify whether to display all calendars, or only those that may be written to. The view controller can be pushed on a navigation stack or presented modally.

Use a delegate that conforms to EKCalendarChooserDelegate to receive callbacks when the user selects calendars or cancels an operation.

## Topics

### Initializing Calendar Choosers

init(selectionStyle: EKCalendarChooserSelectionStyle, displayStyle: EKCalendarChooserDisplayStyle, eventStore: EKEventStore)

Initializes a newly created calendar chooser.

init(selectionStyle: EKCalendarChooserSelectionStyle, displayStyle: EKCalendarChooserDisplayStyle, entityType: EKEntityType, eventStore: EKEventStore)

Initializes a newly created calendar chooser for a specific entity type.

### Managing Calendar Selection

var delegate: (any EKCalendarChooserDelegate)?

The calendar chooser’s delegate.

protocol EKCalendarChooserDelegate

Methods a calendar chooser’s delegate may use to receive notifications.

### Selecting a Calendar Type

var selectedCalendars: Set&lt;EKCalendar>

The calendars selected by the user.

var selectionStyle: EKCalendarChooserSelectionStyle

Determines whether to allow selection of multiple calendars.

enum EKCalendarChooserSelectionStyle

Indicates whether users may select a single calendar, or multiple calendars.

enum EKCalendarChooserDisplayStyle

Indicates whether to display all calendars or writable calendars only.

### Changing the Appearance

var showsCancelButton: Bool

A Boolean that determines whether to display a Cancel button.

var showsDoneButton: Bool

A Boolean that determines whether to display a Done button.

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

