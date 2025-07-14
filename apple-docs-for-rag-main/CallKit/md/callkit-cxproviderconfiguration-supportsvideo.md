

- CallKit
- CXProviderConfiguration
-  supportsVideo 

Instance Property

# supportsVideo

A Boolean value that indicates whether the provider supports video in addition to audio.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+macOS 11.0+visionOS 1.0+watchOS 9.0+

``` source
var supportsVideo: Bool { get set }
```

## Discussion

By default, this property is set to false.

## See Also

### Configuring Call Capabilities

var maximumCallGroups: Int

The maximum number of call groups.

var maximumCallsPerCallGroup: Int

The maximum number of calls per call group.

var supportedHandleTypes: Set&lt;CXHandle.HandleType>

The supported handle types.

var includesCallsInRecents: Bool

A Boolean value that indicates whether the provider includes a call in the system’s Recents list after the call ends.

