

- CallKit
- CXCallUpdate
-  localizedCallerName 

Instance Property

# localizedCallerName

The localized name of the caller.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
var localizedCallerName: String? { get set }
```

## Discussion

By default, the system automatically provides a localized caller name using information like the user’s contacts based on the supplied caller identifier. You can set this property to override the system-provided value.

## See Also

### Accessing Call Update Attributes

var remoteHandle: CXHandle?

The handle for the remote party (for an incoming call, this is the caller; for an outgoing call, this is the callee).

var hasVideo: Bool

A Boolean value that indicates whether the call includes video in addition to audio.

var supportsGrouping: Bool

A Boolean value that indicates whether the call can be grouped with other calls.

var supportsUngrouping: Bool

A Boolean value that indicates whether the call can be ungrouped from other calls.

var supportsHolding: Bool

A Boolean value that indicates whether the call can be placed on hold or removed from hold.

var supportsDTMF: Bool

A Boolean value that indicates whether the call can send DTMF (dual tone multifrequency) tones via hard pause digits or in-call keypad entries.

