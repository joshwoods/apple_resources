

- Multipeer Connectivity
- MCSession
-  Multipeer Connectivity Error Domain 

API Collection

# Multipeer Connectivity Error Domain

The error domain for errors specific to Multipeer Connectivity.

## Topics

### Constants

let MCErrorDomain: String

The `NSError` domain constant. If the `domain` value for an `NSError` object is equal to `MCErrorDomain`, then the error was produced by the Multipeer Connectivity framework itself, as opposed to a lower-level framework on which it depends.

## See Also

### Constants

enum MCSessionSendDataMode

Indicates whether delivery of data should be guaranteed.

enum MCSessionState

Indicates the current state of a given peer within a session.

enum MCEncryptionPreference

Indicates whether a session should use encryption when communicating with nearby peers.

enum Code

Error codes found in MCErrorDomain error domain `NSError` objects returned by methods in the Multipeer Connectivity framework.

Minimum and Maximum Supported Peers

Constants that define the minimum and maximum number of peers supported in a session.

