

- UIKit
-  UIPointerInteractionAnimating 

Protocol

# UIPointerInteractionAnimating

An interface for modifying an interaction animation in coordination with the pointer effect animations.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+visionOS 1.0+

``` source
@MainActor
protocol UIPointerInteractionAnimating : NSObjectProtocol
```

## Topics

### Managing animations

func addAnimations(() -> Void)

Adds the specified animation block to the animator.

**Required**

func addCompletion((Bool) -> Void)

Adds the specified completion block to the animator.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

