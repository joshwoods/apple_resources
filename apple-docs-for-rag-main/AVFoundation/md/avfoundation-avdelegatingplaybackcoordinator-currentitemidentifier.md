

- AVFoundation
- AVDelegatingPlaybackCoordinator
-  currentItemIdentifier 

Instance Property

# currentItemIdentifier

An identifier of the current item.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
var currentItemIdentifier: String? { get }
```

## Discussion

The coordinator sets this value in a previous call to transitionToItem(withIdentifier:proposingInitialTimingBasedOn:).

