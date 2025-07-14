

- CryptoTokenKit
- TKToken
- TKToken.Configuration
-  configurationData 

Instance Property

# configurationData

Additional configuration information for the token instance.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 10.15+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
var configurationData: Data? { get set }
```

## Discussion

configurationData can provide token-implementation-specific additional data, which the app that hosts the token driver extension and configures the token provides. The system doesn’t interpret this data in any way.

For example, the network-based hardware security module (HSM) can store encoded target network addresses, access credentials, or the list of identities the HSM contains.

## See Also

### Reporting Configuration Information

var instanceID: TKToken.InstanceID

The unique, persistent identifier of this token that the token implementation creates.

