

- RealityKit
- NetworkCompatibilityToken
-  compatibilityWith(\_:) 

Instance Method

# compatibilityWith(\_:)

Compares network compatibility tokens between the local device and another device.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOS 10.15.4+visionOS

``` source
final func compatibilityWith(_ otherToken: NetworkCompatibilityToken) -> NetworkCompatibilityToken.Compatibility
```

## Parameters 

`otherToken`  

The token for the remote client against which the local device checks compatibility

## Return Value

Returns NetworkCompatibilityToken.Compatibility.compatible if the local client and the remote client represented by `otherToken` can be synced. Any other result indicates that the two devices are incompatible and you shouldn’t proceed with the connection.

