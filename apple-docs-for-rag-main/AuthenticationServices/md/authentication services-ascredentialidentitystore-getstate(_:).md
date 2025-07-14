

- Authentication Services
- ASCredentialIdentityStore
-  getState(\_:) 

Instance Method

# getState(\_:)

Gets the state of the credential identity store.

iOS 12.0+iPadOS 12.0+Mac Catalyst 14.0+macOS 11.0+visionOS 1.0+

``` source
func getState(_ completion: @escaping (ASCredentialIdentityStoreState) -> Void)
```

``` source
func state() async -> ASCredentialIdentityStoreState
```

## Parameters 

`completion`  

A block the method calls to return the current identity store state.

## Discussion

Call this method to find out the current state of the store before attempting to call other store methods. Examine the ASCredentialIdentityStoreState value passed to your completion handler to find out whether the store is enabled and whether it supports incremental updates.

## See Also

### Checking the state of the store

class ASCredentialIdentityStoreState

A representation of the state of a credential identity store.

