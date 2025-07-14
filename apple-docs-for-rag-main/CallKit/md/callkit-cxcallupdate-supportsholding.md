

- CallKit
- CXCallUpdate
-  supportsHolding 

Instance Property

# supportsHolding

A Boolean value that indicates whether the call can be placed on hold or removed from hold.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
var supportsHolding: Bool { get set }
```

## See Also

### Accessing Call Update Attributes

var localizedCallerName: String?

The localized name of the caller.

var remoteHandle: CXHandle?

The handle for the remote party (for an incoming call, this is the caller; for an outgoing call, this is the callee).

var hasVideo: Bool

A Boolean value that indicates whether the call includes video in addition to audio.

var supportsGrouping: Bool

A Boolean value that indicates whether the call can be grouped with other calls.

var supportsUngrouping: Bool

A Boolean value that indicates whether the call can be ungrouped from other calls.

var supportsDTMF: Bool

A Boolean value that indicates whether the call can send DTMF (dual tone multifrequency) tones via hard pause digits or in-call keypad entries.

