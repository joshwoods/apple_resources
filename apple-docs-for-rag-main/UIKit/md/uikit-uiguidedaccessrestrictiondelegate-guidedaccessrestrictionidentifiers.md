

- UIKit
- UIGuidedAccessRestrictionDelegate
-  guidedAccessRestrictionIdentifiers 

Instance Property

# guidedAccessRestrictionIdentifiers

An array of strings identifying custom restrictions.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var guidedAccessRestrictionIdentifiers: [String]? { get }
```

**Required**

## Return Value

An array of NSString objects, each of which represents a custom restriction.

## Discussion

Your delegate must implement this method and return an array with an identifier string for each custom guided access restriction you wish to provide in your app.

## See Also

### Identifying custom Guided Access restrictions

func textForGuidedAccessRestriction(withIdentifier: String) -> String?

Provides a succinct description of the restriction for the specified identifier.

**Required**

func detailTextForGuidedAccessRestriction(withIdentifier: String) -> String?

Provides more detailed information about the restriction for the specified identifier.

