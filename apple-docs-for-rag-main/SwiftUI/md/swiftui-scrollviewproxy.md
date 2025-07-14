

- SwiftUI
-  ScrollViewProxy 

Structure

# ScrollViewProxy

A proxy value that supports programmatic scrolling of the scrollable views within a view hierarchy.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
struct ScrollViewProxy
```

## Overview

You don’t create instances of `ScrollViewProxy` directly. Instead, your ScrollViewReader receives an instance of `ScrollViewProxy` in its `content` view builder. You use actions within this view builder, such as button and gesture handlers or the onChange(of:perform:) method, to call the proxy’s scrollTo(_:anchor:) method.

## Topics

### Performing scrolling

func scrollTo&lt;ID>(ID, anchor: UnitPoint?)

Scans all scroll views contained by the proxy for the first with a child view with identifier `id`, and then scrolls to that view.

## See Also

### Creating a scroll view

struct ScrollView

A scrollable view.

struct ScrollViewReader

A view that provides programmatic scrolling, by working with a proxy to scroll to known child views.

