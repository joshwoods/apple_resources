

- UIKit
- UIGuidedAccessRestrictionDelegate
-  guidedAccessRestriction(withIdentifier:didChange:) 

Instance Method

# guidedAccessRestriction(withIdentifier:didChange:)

Tells the delegate that the restriction associated with the identifier has changed state.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func guidedAccessRestriction(
    withIdentifier restrictionIdentifier: String,
    didChange newRestrictionState: UIAccessibility.GuidedAccessRestrictionState
)
```

**Required**

## Parameters 

`restrictionIdentifier`  

The identifier of the restriction whose state has changed.

`newRestrictionState`  

The new state for the restriction.

## Discussion

Your app should adjust its behavior to allow or deny the operation controlled by the specified restriction each time it receives this message.

## See Also

### Implementing restrictions

enum GuidedAccessRestrictionState

Constants that describe the state of a restriction, either allow or deny.

