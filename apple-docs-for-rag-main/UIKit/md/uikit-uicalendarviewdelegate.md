

- UIKit
-  UICalendarViewDelegate 

Protocol

# UICalendarViewDelegate

An object that a calendar view uses to display decorations for dates.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
protocol UICalendarViewDelegate : NSObjectProtocol
```

## Topics

### Providing calendar view decorations

func calendarView(UICalendarView, decorationFor: DateComponents) -> UICalendarView.Decoration?

Creates a calendar view decoration for the date represented by the date components you provide.

### Instance Methods

func calendarView(UICalendarView, didChangeVisibleDateComponentsFrom: DateComponents)

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Customizing the calendar display

var fontDesign: UIFontDescriptor.SystemDesign

A font design that the calendar view uses for displaying calendar text.

var delegate: (any UICalendarViewDelegate)?

A delegate object the calendar view calls for decoration views.

class Decoration

A view that a calendar view displays for a specific date.

enum DecorationSize

Constants that indicate the relative size of a decoration in a calendar view.

var wantsDateDecorations: Bool

A Boolean value that indicates whether the calendar view displays date decorations.

func reloadDecorations(forDateComponents: [DateComponents], animated: Bool)

Reloads the decorations for the dates you provide, with an option to animate the decoration reload.

