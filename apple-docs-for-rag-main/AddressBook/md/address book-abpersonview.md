

- Address Book
-  ABPersonView 

Class

# ABPersonView

An object that provides a view for displaying and editing contacts.

macOS 10.7+

``` source
@MainActor
class ABPersonView
```

## Overview

Note

You should not override the fieldEditor(_:for:) method of the window that contains this view.

## Topics

### Working with Person Views

var editing: Bool

A Boolean value that indicates whether the person view is in editing mode.

var person: ABPerson!

The contact record being displayed.

var shouldShowLinkedPeople: Bool

Indicates whether the person view should display data from person records that are linked with the person record being displayed.

## Relationships

### Inherits From

- NSView

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSAccessibilityElementProtocol
- NSAccessibilityProtocol
- NSAnimatablePropertyContainer
- NSAppearanceCustomization
- NSCoding
- NSDraggingDestination
- NSObjectProtocol
- NSStandardKeyBindingResponding
- NSTouchBarProvider
- NSUserActivityRestoring
- NSUserInterfaceItemIdentification
- Sendable

## See Also

### Pickers

class ABPeoplePickerView

An object you use to customize the behavior of people-picker views in an app’s user interface.

