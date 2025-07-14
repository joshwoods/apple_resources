

- UIKit
- UICalendarView
-  reloadDecorations(forDateComponents:animated:) 

Instance Method

# reloadDecorations(forDateComponents:animated:)

Reloads the decorations for the dates you provide, with an option to animate the decoration reload.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
func reloadDecorations(
    forDateComponents dates: [DateComponents],
    animated: Bool
)
```

## Parameters 

`dates`  

An array of dates to reload that you provide as date components.

`animated`  

A Boolean value that indicates whether the calendar view should animate the decoration reload.

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

var wantsDateDecorations: Bool

A Boolean value that indicates whether the calendar view displays date decorations.

