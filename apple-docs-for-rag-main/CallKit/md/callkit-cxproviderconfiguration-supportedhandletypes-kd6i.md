

- CallKit
- CXProviderConfiguration
-  supportedHandleTypes 

Instance Property

# supportedHandleTypes

The supported handle types.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
@nonobjc
final var supportedHandleTypes: Set { get set }
```

## Discussion

For possible values, see CXHandle.HandleType.

## See Also

### Configuring Call Capabilities

var maximumCallGroups: Int

The maximum number of call groups.

var maximumCallsPerCallGroup: Int

The maximum number of calls per call group.

var supportsVideo: Bool

A Boolean value that indicates whether the provider supports video in addition to audio.

var includesCallsInRecents: Bool

A Boolean value that indicates whether the provider includes a call in the system’s Recents list after the call ends.

