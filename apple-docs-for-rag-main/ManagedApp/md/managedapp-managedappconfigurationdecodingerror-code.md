

- ManagedApp
- ManagedAppConfigurationDecodingError
-  code 

Instance Property

# code

An app-specific error code that identifies a configuration issue.

iOS 18.4+iPadOS 18.4+visionOS 2.4+

``` source
var code: ManagedAppConfigurationDecodingErrorCode { get set }
```

**Required**

## Mentioned in 

Specifying and decoding a configuration

## Discussion

The system reserves values equal to or greater than `ManagedAppConfigurationDecodingErrorCodes.firstReserved`.

