

- ContactProvider
- ContactProviderManager
-  enable() 

Instance Method

# enable()

Requests the person using the app to enable the extension domain.

iOS 18.0+iPadOS 18.0+

``` source
func enable() async throws
```

## Discussion

If necessary, this call waits for the person using the app to explicitly approve or deny using the extension domain.

Throws

`ContactProviderError.deniedByUser` if the person dismisses the prompt without enabling the extension domain.

## See Also

### Managing the domain

var domain: any ContactProviderDomain

The domain that this instance manages.

var isEnabled: Bool

A Boolean value that indicates whether the person using the app enabled the extension domain.

func reset() async throws

Resets the extension domain.

func disable() async throws

Disables the extension domain.

