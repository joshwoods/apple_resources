

- ARKit
- ARCoachingOverlayView
-  delegate 

Instance Property

# delegate

An object you supply that implements coaching event callbacks.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
@IBOutlet @MainActor
weak var delegate: (any ARCoachingOverlayViewDelegate)? { get set }
```

## Discussion

Normally, you set the value of this property to your app’s view controller.

## See Also

### Delegating Events

protocol ARCoachingOverlayViewDelegate

A set of callbacks you implement to be notified of coaching events.

