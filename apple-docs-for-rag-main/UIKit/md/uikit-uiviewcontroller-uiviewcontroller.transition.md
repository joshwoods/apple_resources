

- UIKit
- UIViewController
-  UIViewController.Transition 

Class

# UIViewController.Transition

An object that defines the transition animation when switching to a new view controller.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+tvOS 18.0+visionOS 2.0+

``` source
class Transition
```

## Topics

### Creating zoom transitions

static func zoom(options: UIViewController.Transition.ZoomOptions?, sourceViewProvider: (UIViewController.Transition.ZoomSourceViewProviderContext) -> UIView?) -> Self

Creates a zoom transition from the view that the source provider specifies.

class ZoomOptions

Options for a zoom transition.

class ZoomSourceViewProviderContext

A context object that contains references to the view controllers from a zoom transition.

### Accessing transitions

static var coverVertical: Self

A transition where the new view slides up from the bottom of the screen.

static var crossDissolve: Self

A transition where the current view fades out while the new view fades in at the same time.

static var flipHorizontal: Self

A transition where the current view flips horizontally to reveal the new view.

static var partialCurl: Self

A transition where one corner of the current view curls up, revealing the new view underneath.

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

## See Also

### Working with transitions

var preferredTransition: UIViewController.Transition?

An object that defines the transition animation when switching to the view controller.

