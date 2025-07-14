

- Authentication Services
- ASAuthorizationProviderExtensionRegistrationResult
-  ASAuthorizationProviderExtensionRegistrationResult.userInterfaceRequired 

Case

# ASAuthorizationProviderExtensionRegistrationResult.userInterfaceRequired

The user interface is required to complete registration.

macOS 13.0+

``` source
case userInterfaceRequired
```

## See Also

### Identifying the results

case failed

The registration fails to complete and the system retries later.

case failedNoRetry

The registration fails to complete and the system doesn’t retry later.

case success

The registration succeeds.

