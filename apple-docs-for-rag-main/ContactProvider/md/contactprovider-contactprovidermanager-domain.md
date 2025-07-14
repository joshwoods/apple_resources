

- ContactProvider
- ContactProviderManager
-  domain 

Instance Property

# domain

The domain that this instance manages.

iOS 18.0+iPadOS 18.0+

``` source
var domain: any ContactProviderDomain { get }
```

## Discussion

This value defaults to DefaultContactProviderDomain.

## See Also

### Managing the domain

func enable() async throws

Requests the person using the app to enable the extension domain.

var isEnabled: Bool

A Boolean value that indicates whether the person using the app enabled the extension domain.

func reset() async throws

Resets the extension domain.

func disable() async throws

Disables the extension domain.

