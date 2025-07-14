

- Network
- NWParameters
-  setPrivacyContext(\_:) 

Instance Method

# setPrivacyContext(\_:)

Associates a privacy context with any connections or listeners that use the parameters.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
final func setPrivacyContext(_ privacyContext: NWParameters.PrivacyContext)
```

## Discussion

The privacy context allows using separate caches for different sets of connections, as well as restricting how connection-specific information is logged and shared on the network.

## See Also

### Configuring Privacy Settings

class PrivacyContext

An object that defines the privacy requirements for a set of connections.

