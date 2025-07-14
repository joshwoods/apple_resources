

- Multipeer Connectivity
- MCEncryptionPreference
-  MCEncryptionPreference.optional 

Case

# MCEncryptionPreference.optional

The session prefers to use encryption, but accepts unencrypted connections. A connection uses encryption when all the peers choose either MCEncryptionPreference.optional or MCEncryptionPreference.required. If some peers choose MCEncryptionPreference.none, then the session will not be encrypted. For this reason, if some peers running your app can be configured without encryption, you should always assume that the session is unencrypted.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 10.0+visionOS 1.0+

``` source
case optional
```

## See Also

### Constants

case required

The session requires encryption.

case none

The session should not be encrypted.

