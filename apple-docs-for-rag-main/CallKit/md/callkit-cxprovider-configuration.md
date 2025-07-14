

- CallKit
- CXProvider
-  configuration 

Instance Property

# configuration

The configuration of the provider.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
@NSCopying
var configuration: CXProviderConfiguration { get set }
```

## Discussion

This property returns a copy of the provider configuration. To change the configuration of the provider, you must set this property to a new CXProviderConfiguration object.

