

- Authentication Services
- ASAuthorizationProviderExtensionLoginManager
-  resetKeys() 

Instance Method

# resetKeys()

Creates new encryption, signing, and Secure Enclave keys for the user.

macOS 13.0+

``` source
func resetKeys()
```

## Discussion

This call permanently destroys the keys and you can’t undo it.

## See Also

### Repairing registrations

func userRegistrationsNeedsRepair()

Invokes the user registration to run again so the current user can repair it.

func deviceRegistrationsNeedsRepair()

Invokes the device registration to run again so the current user can repair it.

