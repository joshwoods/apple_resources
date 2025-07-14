

- ContactProvider
- ContactProviderManager
-  init(domainIdentifier:) 

Initializer

# init(domainIdentifier:)

Creates a provider manager.

iOS 18.0+iPadOS 18.0+

``` source
init(domainIdentifier: String = DefaultContactProviderDomain.identifier) throws
```

## Parameters 

`domainIdentifier`  

A string to identify a domain of contacts to provide. Defaults to identifier.

## Discussion

If needed, the manager registers the DefaultContactProviderDomain for the extension.

Throws

ContactProviderError.extensionNotFound if discovering the extension fails.

Throws

ContactProviderError.featureNotAvailable when running on an unsupported platform.

