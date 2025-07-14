

- CloudKit
- CKDiscoverAllUserIdentitiesOperation
-  discoverAllUserIdentitiesCompletionBlock Deprecated

Instance Property

# discoverAllUserIdentitiesCompletionBlock

The closure to execute when the operation finishes.

iOS 10.0–15.0DeprecatediPadOS 10.0–15.0DeprecatedMac Catalyst 13.1–15.0DeprecatedmacOS 10.12–12.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–8.0Deprecated

``` source
var discoverAllUserIdentitiesCompletionBlock: (((any Error)?) -> Void)? { get set }
```

Deprecated

Use discoverAllUserIdentitiesResultBlock instead

## Discussion

The closure doesn’t return a value and takes the following parameter:

- An error if a problem occurs, or `nil` if CloudKit successfully fetches the user identities.

This closure executes only once, after all of the individual discovery closures finish. The closure executes serially with respect to the operation’s other closures. If you intend to use this closure to process results, update the property’s value before you execute the operation or submit it to a queue.

## See Also

### Processing the Operation Results

var userIdentityDiscoveredBlock: ((CKUserIdentity) -> Void)?

The closure to execute for each user identity.

Deprecated

