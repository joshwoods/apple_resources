

- UIKit
- UICalendarView
-  UICalendarView.Decoration 

Class

# UICalendarView.Decoration

A view that a calendar view displays for a specific date.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
class Decoration
```

## Topics

### Creating a Default Decoration View

init()

Creates a default calendar view decoration with a filled circle image, using the system fill color and medium size.

static func `default`(color: UIColor?, size: UICalendarView.DecorationSize) -> UICalendarView.Decoration

Creates a default calendar view decoration with a filled circle image, using the color and size you specify.

### Creating a Custom Decoration View

class func customView(() -> UIView) -> Self

Creates a new calendar view decoration with a custom view, using your view provider.

### Creating Image Decoration Views

static func image(UIImage?, color: UIColor?, size: UICalendarView.DecorationSize) -> UICalendarView.Decoration

Creates a new calendar view decoration with the image, color, and size that you specify.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Customizing the calendar display

var fontDesign: UIFontDescriptor.SystemDesign

A font design that the calendar view uses for displaying calendar text.

var delegate: (any UICalendarViewDelegate)?

A delegate object the calendar view calls for decoration views.

protocol UICalendarViewDelegate

An object that a calendar view uses to display decorations for dates.

enum DecorationSize

Constants that indicate the relative size of a decoration in a calendar view.

var wantsDateDecorations: Bool

A Boolean value that indicates whether the calendar view displays date decorations.

func reloadDecorations(forDateComponents: [DateComponents], animated: Bool)

Reloads the decorations for the dates you provide, with an option to animate the decoration reload.

