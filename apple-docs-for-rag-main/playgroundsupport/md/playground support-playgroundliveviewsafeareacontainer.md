

- Playground Support
-  PlaygroundLiveViewSafeAreaContainer 

Protocol

# PlaygroundLiveViewSafeAreaContainer

A protocol that ensures that views fit without obstruction within the Swift Playgrounds user interface.

Xcode 10.2+Swift Playgrounds 2.0+

``` source
protocol PlaygroundLiveViewSafeAreaContainer : AnyObject
```

## Overview

This protocol provides liveViewSafeAreaGuide, a layout guide set to the safe area. The *safe area* is the part of the live view that isn't covered by any Swift Playgrounds user interface elements like the Run button. You use this property to constrain the bounds of your content view inside the bounds of the safe area, which depend on how you set the `LiveViewEdgeToEdge` key for the current page. When this key is set to `NO`, the safe area is exactly the same as the live view area. When the key is set to `YES`, the safe area can be smaller than the live view area.

## Topics

### Accessing the Layout Guide

var liveViewSafeAreaGuide: UILayoutGuide

A layout guide you use to position content so that it's unobstructed by the Swift Playgrounds user interface.

**Required** Default implementations provided.

Deprecated

## See Also

### Live Views

protocol PlaygroundLiveViewable

A protocol that displays an instance as a live view in a playground.

enum PlaygroundLiveViewRepresentation

The supported types for displaying for live views in playgrounds.

