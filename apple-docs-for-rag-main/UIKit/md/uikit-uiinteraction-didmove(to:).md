

- UIKit
- UIInteraction
-  didMove(to:) 

Instance Method

# didMove(to:)

Tells the interaction that a view added or removed it from the view’s interactions array.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
func didMove(to view: UIView?)
```

**Required**

## Parameters 

`view`  

The view that owns and contains the interaction in its interaction array. If the view is `nil`, the interaction’s owner removed the interaction from its interactions array.

## See Also

### Tracking the Movements

func willMove(to: UIView?)

Tells the interaction that a view will add or remove it from the view’s interactions array.

**Required**

