

- UIKit
-  UITransitionContextViewControllerKey 

Structure

# UITransitionContextViewControllerKey

The keys you use to identify the view controllers involved in a transition.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
struct UITransitionContextViewControllerKey
```

## Topics

### Keys

static let from: UITransitionContextViewControllerKey

A key that identifies the view controller that’s visible at the beginning of the transition, or at the end of a canceled transition.

static let to: UITransitionContextViewControllerKey

A key that identifies the view controller that’s visible at the end of a completed transition.

### Initializers

init(rawValue: String)

Creates a key to identify the view controllers in a transition.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

struct UITransitionContextViewKey

The keys you use to identify the views involved in a transition.

