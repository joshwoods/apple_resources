

- CloudKit
- CKDiscoverAllUserIdentitiesOperation
-  userIdentityDiscoveredBlock Deprecated

Instance Property

# userIdentityDiscoveredBlock

The closure to execute for each user identity.

iOS 10.0–17.0DeprecatediPadOS 10.0–17.0DeprecatedMac Catalyst 13.1–17.0DeprecatedmacOS 10.12–14.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–10.0Deprecated

``` source
var userIdentityDiscoveredBlock: ((CKUserIdentity) -> Void)? { get set }
```

Deprecated

No longer supported. Please see Sharing CloudKit Data with Other iCloud Users.

## Discussion

The closure doesn’t return a value and takes the following parameter:

- The user identity that matches an entry in the device’s Contacts.

The operation executes this closure one or more times for each user identity it discovers. Each time the closure executes, it executes serially with respect to the other closures of the operation.

If you intend to use this closure to process results, set it before you execute the operation or add the operation to a queue.

## See Also

### Processing the Operation Results

var discoverAllUserIdentitiesCompletionBlock: (((any Error)?) -> Void)?

The closure to execute when the operation finishes.

Deprecated

