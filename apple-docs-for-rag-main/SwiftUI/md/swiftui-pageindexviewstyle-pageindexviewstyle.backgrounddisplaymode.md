

- SwiftUI
- PageIndexViewStyle
-  PageIndexViewStyle.BackgroundDisplayMode 

Structure

# PageIndexViewStyle.BackgroundDisplayMode

The background style for the page index view.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+watchOS 8.0+

``` source
struct BackgroundDisplayMode
```

## Topics

### Getting the display modes

static let automatic: PageIndexViewStyle.BackgroundDisplayMode

Background will use the default for the platform.

static let always: PageIndexViewStyle.BackgroundDisplayMode

Background is always displayed behind the page index view.

static let interactive: PageIndexViewStyle.BackgroundDisplayMode

Background is only shown while the index view is interacted with.

static let never: PageIndexViewStyle.BackgroundDisplayMode

Background is never displayed behind the page index view.

## Relationships

### Conforms To

- Sendable

## See Also

### Creating the control group style

init(backgroundDisplayMode: PageIndexViewStyle.BackgroundDisplayMode)

Creates a page index view style.

