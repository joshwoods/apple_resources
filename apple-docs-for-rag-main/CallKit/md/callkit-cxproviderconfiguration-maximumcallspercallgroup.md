

- CallKit
- CXProviderConfiguration
-  maximumCallsPerCallGroup 

Instance Property

# maximumCallsPerCallGroup

The maximum number of calls per call group.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+macOS 11.0+visionOS 1.0+watchOS 9.0+

``` source
var maximumCallsPerCallGroup: Int { get set }
```

## Discussion

By default, the maximum number is `5`.

## See Also

### Configuring Call Capabilities

var maximumCallGroups: Int

The maximum number of call groups.

var supportedHandleTypes: Set&lt;CXHandle.HandleType>

The supported handle types.

var supportsVideo: Bool

A Boolean value that indicates whether the provider supports video in addition to audio.

var includesCallsInRecents: Bool

A Boolean value that indicates whether the provider includes a call in the system’s Recents list after the call ends.

