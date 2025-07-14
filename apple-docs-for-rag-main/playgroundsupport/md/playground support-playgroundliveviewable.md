

- Playground Support
-  PlaygroundLiveViewable 

Protocol

# PlaygroundLiveViewable

A protocol that displays an instance as a live view in a playground.

macOS 11.0+Xcode 10.2+Swift Playgrounds 2.0+

``` source
protocol PlaygroundLiveViewable
```

## Overview

A playground that presents a simplified user interface programming environment, for example, can make its view-like type conform to `PlaygroundLiveViewable` and appear in the live view. By default, UIView and UIViewController conform to this protocol in iOS and tvOS, and NSView and NSViewController conform to this protocol in macOS. You only need to implement this protocol for custom objects that don't already inherit from UIView, UIViewController, NSView, or NSViewController.

## Topics

### Displaying Types

var playgroundLiveViewRepresentation: PlaygroundLiveViewRepresentation

The view or view controller used to render and manage the live view.

**Required**

## Relationships

### Conforming Types

- PlaygroundRemoteLiveViewProxy

## See Also

### Live Views

enum PlaygroundLiveViewRepresentation

The supported types for displaying for live views in playgrounds.

protocol PlaygroundLiveViewSafeAreaContainer

A protocol that ensures that views fit without obstruction within the Swift Playgrounds user interface.

