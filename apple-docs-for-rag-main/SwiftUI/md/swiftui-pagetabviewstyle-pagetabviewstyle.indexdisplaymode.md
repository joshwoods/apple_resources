

- SwiftUI
- PageTabViewStyle
-  PageTabViewStyle.IndexDisplayMode 

Structure

# PageTabViewStyle.IndexDisplayMode

A style for displaying the page index view

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
struct IndexDisplayMode
```

## Topics

### Getting the modes

static let always: PageTabViewStyle.IndexDisplayMode

Always display an index view regardless of page count

static let automatic: PageTabViewStyle.IndexDisplayMode

Displays an index view when there are more than one page

static let never: PageTabViewStyle.IndexDisplayMode

Never display an index view

## Relationships

### Conforms To

- Sendable

## See Also

### Creating a page tab view style

init(indexDisplayMode: PageTabViewStyle.IndexDisplayMode)

Creates a new `PageTabViewStyle` with an index display mode

