

- UIKit
- UIGuidedAccessRestrictionDelegate
-  textForGuidedAccessRestriction(withIdentifier:) 

Instance Method

# textForGuidedAccessRestriction(withIdentifier:)

Provides a succinct description of the restriction for the specified identifier.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func textForGuidedAccessRestriction(withIdentifier restrictionIdentifier: String) -> String?
```

**Required**

## Parameters 

`restrictionIdentifier`  

The identifer of the restriction the system is interested in.

## Return Value

A localized, human-readable string that succinctly describes the restriction for the provided identifier.

## See Also

### Identifying custom Guided Access restrictions

var guidedAccessRestrictionIdentifiers: [String]?

An array of strings identifying custom restrictions.

**Required**

func detailTextForGuidedAccessRestriction(withIdentifier: String) -> String?

Provides more detailed information about the restriction for the specified identifier.

