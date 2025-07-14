

- SwiftUI
- VerticalPageTabViewStyle
-  VerticalPageTabViewStyle.TransitionStyle 

Structure

# VerticalPageTabViewStyle.TransitionStyle

A transition style used between tabs.

watchOS 10.0+

``` source
struct TransitionStyle
```

## Topics

### Getting the transition styles

static let automatic: VerticalPageTabViewStyle.TransitionStyle

Automatic transition style

static let blur: VerticalPageTabViewStyle.TransitionStyle

A transition style that blurs content between each tab

static let identity: VerticalPageTabViewStyle.TransitionStyle

A transition style that has no animation between each tab

## See Also

### Creating the tab view style

init()

init(transitionStyle: VerticalPageTabViewStyle.TransitionStyle)

Creates a new `VerticalPageTabViewStyle` with a transition style.

