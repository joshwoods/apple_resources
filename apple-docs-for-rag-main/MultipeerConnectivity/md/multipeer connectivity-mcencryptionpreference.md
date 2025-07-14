

- Multipeer Connectivity
-  MCEncryptionPreference 

Enumeration

# MCEncryptionPreference

Indicates whether a session should use encryption when communicating with nearby peers.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 10.0+visionOS 1.0+

``` source
enum MCEncryptionPreference
```

## Topics

### Constants

case optional

The session prefers to use encryption, but accepts unencrypted connections. A connection uses encryption when all the peers choose either MCEncryptionPreference.optional or MCEncryptionPreference.required. If some peers choose MCEncryptionPreference.none, then the session will not be encrypted. For this reason, if some peers running your app can be configured without encryption, you should always assume that the session is unencrypted.

case required

The session requires encryption.

case none

The session should not be encrypted.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Constants

enum MCSessionSendDataMode

Indicates whether delivery of data should be guaranteed.

enum MCSessionState

Indicates the current state of a given peer within a session.

enum Code

Error codes found in MCErrorDomain error domain `NSError` objects returned by methods in the Multipeer Connectivity framework.

Multipeer Connectivity Error Domain

The error domain for errors specific to Multipeer Connectivity.

Minimum and Maximum Supported Peers

Constants that define the minimum and maximum number of peers supported in a session.

