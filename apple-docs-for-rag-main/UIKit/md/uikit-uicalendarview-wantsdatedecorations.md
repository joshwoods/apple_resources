

- UIKit
- UICalendarView
-  wantsDateDecorations 

Instance Property

# wantsDateDecorations

A Boolean value that indicates whether the calendar view displays date decorations.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
var wantsDateDecorations: Bool { get set }
```

## Discussion

Defaults to true. You must implement `UICalendarDateDelegate`’s calendarView(_:decorationFor:) to provide decorations that the calendar view shows.

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

enum DecorationSize

Constants that indicate the relative size of a decoration in a calendar view.

func reloadDecorations(forDateComponents: [DateComponents], animated: Bool)

Reloads the decorations for the dates you provide, with an option to animate the decoration reload.

