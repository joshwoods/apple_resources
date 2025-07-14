

- Authentication Services
- ASCredentialIdentityStoreState
-  supportsIncrementalUpdates 

Instance Property

# supportsIncrementalUpdates

A Boolean value indicating whether the credential identity store supports incremental updates.

iOS 12.0+iPadOS 12.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
var supportsIncrementalUpdates: Bool { get }
```

## Discussion

Examine the value returned by this property to find out if the credential identity store can accept incremental updates. If incremental updates are supported, you can update the credential identity store with only the new changes since the last time it was updated. Otherwise, update the credential identity store by adding all credential identities.

## See Also

### Checking the state

var isEnabled: Bool

A Boolean value indicating whether the credential identity store is enabled.

