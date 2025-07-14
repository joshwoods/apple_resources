

- RealityKit
- NetworkCompatibilityToken
- NetworkCompatibilityToken.Compatibility
-  NetworkCompatibilityToken.Compatibility.sessionProtocolVersionMismatch 

Case

# NetworkCompatibilityToken.Compatibility.sessionProtocolVersionMismatch

An indication that two peers running incompatible versions of RealityKit can’t sync.

iOS 13.4+iPadOS 13.4+Mac Catalyst 13.4+macOS 10.15.4+visionOS

``` source
case sessionProtocolVersionMismatch
```

## Discussion

The compatibilityWith(_:) method returns this value when two devices have different OS versions and there has been a significant change in networking protocol between those releases.

## See Also

### Compatibility indicators

case compatible

An indication that the compared devices are running compatible versions of RealityKit.

