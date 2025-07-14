

- UIKit
- UICalendarView
-  UICalendarView.DecorationSize 

Enumeration

# UICalendarView.DecorationSize

Constants that indicate the relative size of a decoration in a calendar view.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
enum DecorationSize
```

## Topics

### Decoration View Sizes

case large

A large relative decoration size in a calendar view.

case medium

A medium relative decoration size in a calendar view.

case small

A small relative decoration size in a calendar view.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Customizing the calendar display

var fontDesign: UIFontDescriptor.SystemDesign

A font design that the calendar view uses for displaying calendar text.

var delegate: (any UICalendarViewDelegate)?

A delegate object the calendar view calls for decoration views.

protocol UICalendarViewDelegate

An object that a calendar view uses to display decorations for dates.

class Decoration

A view that a calendar view displays for a specific date.

var wantsDateDecorations: Bool

A Boolean value that indicates whether the calendar view displays date decorations.

func reloadDecorations(forDateComponents: [DateComponents], animated: Bool)

Reloads the decorations for the dates you provide, with an option to animate the decoration reload.

