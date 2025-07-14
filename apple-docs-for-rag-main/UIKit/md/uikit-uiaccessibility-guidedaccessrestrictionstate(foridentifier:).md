

- UIKit
- UIAccessibility
-  guidedAccessRestrictionState(forIdentifier:) 

Type Method

# guidedAccessRestrictionState(forIdentifier:)

Returns the restriction state for the specified guided access restriction.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
static func guidedAccessRestrictionState(forIdentifier restrictionIdentifier: String) -> UIAccessibility.GuidedAccessRestrictionState
```

## Parameters 

`restrictionIdentifier`  

The string that uniquely identifies the guided access restriction.

## Return Value

The current state of the guided access restriction. The initial state of all restrictions is UIAccessibility.GuidedAccessRestrictionState.allow.

## See Also

### Guided Access

protocol UIGuidedAccessRestrictionDelegate

A set of methods you use to add custom restrictions for the Guided Access feature in iOS.

