

- UIKit
- UIGuidedAccessRestrictionDelegate
-  detailTextForGuidedAccessRestriction(withIdentifier:) 

Instance Method

# detailTextForGuidedAccessRestriction(withIdentifier:)

Provides more detailed information about the restriction for the specified identifier.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
optional func detailTextForGuidedAccessRestriction(withIdentifier restrictionIdentifier: String) -> String?
```

## Parameters 

`restrictionIdentifier`  

The identifer of the restriction the system is interested in.

## Return Value

A localized, human-readable string that provides additional information about the restriction for the provided identifier.

## See Also

### Identifying custom Guided Access restrictions

var guidedAccessRestrictionIdentifiers: [String]?

An array of strings identifying custom restrictions.

**Required**

func textForGuidedAccessRestriction(withIdentifier: String) -> String?

Provides a succinct description of the restriction for the specified identifier.

**Required**

