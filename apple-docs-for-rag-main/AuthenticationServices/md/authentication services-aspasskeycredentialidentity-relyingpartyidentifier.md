

- Authentication Services
- ASPasskeyCredentialIdentity
-  relyingPartyIdentifier 

Instance Property

# relyingPartyIdentifier

A string that identifies this identity’s relying party.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+visionOS 1.0+

``` source
var relyingPartyIdentifier: String { get }
```

## Discussion

A passkey credential identity reports its `relyingPartyIdentifier` value as its serviceIdentifier.

