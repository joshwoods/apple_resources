

- UIKit
-  UIGuidedAccessRestrictionDelegate 

Protocol

# UIGuidedAccessRestrictionDelegate

A set of methods you use to add custom restrictions for the Guided Access feature in iOS.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
protocol UIGuidedAccessRestrictionDelegate : NSObjectProtocol
```

## Overview

Custom restrictions are represented by string identifiers provided by the developer in the guidedAccessRestrictionIdentifiers method. Each identifier represents an operation in the app that the developer wishes to allow users to restrict using Guided Access. The default for all operations is allow. Users can deny operations using the normal Guided Access user interface. See http://support.apple.com/kb/HT5509 for a description of how to enable and configure Guided Access on iOS.

Apps describe their custom restrictions by implementing the textForGuidedAccessRestriction(withIdentifier:) and detailTextForGuidedAccessRestriction(withIdentifier:) methods to return appropriate localized, human-readable strings.

For example, a photo editing app might allow users to disable deleting photos. The app would return an identifier representing this restriction in its guidedAccessRestrictionIdentifiers method. It would also implement textForGuidedAccessRestriction(withIdentifier:) to provide a human-readable description of the restriction. Finally, the app would implement guidedAccessRestriction(withIdentifier:didChange:) to notice when a user indicates that they want to enable the restriction. When the app sees the state change to “deny”, it would configure itself to prevent the deletion of photos by any means. Similarly, when the app sees the state change to “allow”, it would configure itself to allow photo deletion.

Apps can use the guidedAccessRestrictionState(forIdentifier:) function to check the state of a restriction at any time.

## Topics

### Identifying custom Guided Access restrictions

var guidedAccessRestrictionIdentifiers: [String]?

An array of strings identifying custom restrictions.

**Required**

func textForGuidedAccessRestriction(withIdentifier: String) -> String?

Provides a succinct description of the restriction for the specified identifier.

**Required**

func detailTextForGuidedAccessRestriction(withIdentifier: String) -> String?

Provides more detailed information about the restriction for the specified identifier.

### Implementing restrictions

func guidedAccessRestriction(withIdentifier: String, didChange: UIAccessibility.GuidedAccessRestrictionState)

Tells the delegate that the restriction associated with the identifier has changed state.

**Required**

enum GuidedAccessRestrictionState

Constants that describe the state of a restriction, either allow or deny.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Guided Access

static func guidedAccessRestrictionState(forIdentifier: String) -> UIAccessibility.GuidedAccessRestrictionState

Returns the restriction state for the specified guided access restriction.

