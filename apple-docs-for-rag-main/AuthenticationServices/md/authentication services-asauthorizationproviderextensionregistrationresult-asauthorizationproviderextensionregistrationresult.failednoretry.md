

- Authentication Services
- ASAuthorizationProviderExtensionRegistrationResult
-  ASAuthorizationProviderExtensionRegistrationResult.failedNoRetry 

Case

# ASAuthorizationProviderExtensionRegistrationResult.failedNoRetry

The registration fails to complete and the system doesn’t retry later.

macOS 13.0+

``` source
case failedNoRetry
```

## Mentioned in 

Registering devices and users

## Discussion

The system attemps to reregister when the mobile device management (MDM) profile changes, or the extension updates.

## See Also

### Identifying the results

case failed

The registration fails to complete and the system retries later.

case success

The registration succeeds.

case userInterfaceRequired

The user interface is required to complete registration.

