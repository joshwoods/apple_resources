

- UIKit
-  UITransitionContextViewKey 

Structure

# UITransitionContextViewKey

The keys you use to identify the views involved in a transition.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
struct UITransitionContextViewKey
```

## Topics

### Keys

static let from: UITransitionContextViewKey

A key that identifies the view shown at the beginning of the transition, or at the end of a canceled transition.

static let to: UITransitionContextViewKey

A key that identifies the view shown at the end of a completed transition.

### Initializers

init(rawValue: String)

Creates a key to identify the views in a transition.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

struct UITransitionContextViewControllerKey

The keys you use to identify the view controllers involved in a transition.

