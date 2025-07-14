

- Network Extension
- NEHotspotEAPSettings
-  setIdentity(\_:) 

Instance Method

# setIdentity(\_:)

Sets the client identity for EAP authentication.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
func setIdentity(_ identity: SecIdentity) -> Bool
```

## Parameters 

`identity`  

The EAP peer identity, a `SecIdentityRef` object that contains a `SecKeyRef` object and an associated `SecCertificateRef` object.

## Return Value

Returns `false` if the parameter is not an object of `SecIdentityRef` type or if the persistent reference is not found in the application’s keychain; otherwise returns `true`.

## Discussion

Your app must store `SecIdentity` in the keychain access group \$`(Team​Identifier​Prefix)com​.apple​.networkextensionsharing`. The OS uses SecItemCopyMatching(_:_:) to obtain a persistent reference to this identity from the application’s keychain and uses it during EAP authentication.

## See Also

### Setting Keychain-based EAP Properties

func setTrustedServerCertificates([Any]) -> Bool

Sets trusted EAP server certificates for an enterprise Wi-Fi or Hotspot 2.0 network.

