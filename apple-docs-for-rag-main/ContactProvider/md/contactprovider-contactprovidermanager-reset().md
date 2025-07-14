

- ContactProvider
- ContactProviderManager
-  reset() 

Instance Method

# reset()

Resets the extension domain.

iOS 18.0+iPadOS 18.0+

``` source
func reset() async throws
```

## Discussion

You typically call this when you need to delete all previously-provided contacts for the domain. The next invocation of the app extension restarts content enumeration for the domain.

## See Also

### Managing the domain

var domain: any ContactProviderDomain

The domain that this instance manages.

func enable() async throws

Requests the person using the app to enable the extension domain.

var isEnabled: Bool

A Boolean value that indicates whether the person using the app enabled the extension domain.

func disable() async throws

Disables the extension domain.

