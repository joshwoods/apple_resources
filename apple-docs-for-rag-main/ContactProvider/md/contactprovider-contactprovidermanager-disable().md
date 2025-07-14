

- ContactProvider
- ContactProviderManager
-  disable() 

Instance Method

# disable()

Disables the extension domain.

iOS 18.0+iPadOS 18.0+

``` source
func disable() async throws
```

## Discussion

Disabling the extension deletes all previously-provided contacts for the domain.

## See Also

### Managing the domain

var domain: any ContactProviderDomain

The domain that this instance manages.

func enable() async throws

Requests the person using the app to enable the extension domain.

var isEnabled: Bool

A Boolean value that indicates whether the person using the app enabled the extension domain.

func reset() async throws

Resets the extension domain.

