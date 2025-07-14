

- Network Extension
- NEHotspotEAPSettings
-  setTrustedServerCertificates(\_:) 

Instance Method

# setTrustedServerCertificates(\_:)

Sets trusted EAP server certificates for an enterprise Wi-Fi or Hotspot 2.0 network.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
func setTrustedServerCertificates(_ certificates: [Any]) -> Bool
```

## Parameters 

`certificates`  

An array of SecCertificate objects. The EAP peer uses these certificates to evaluate the trust of the server certificate chain.

## Return Value

Returns false if any element in the array is not an object of type SecCertificate or if the OS fails to find a persistent reference for each element from the application’s keychain; else return true.

## Discussion

Your app must store the certificates in keychain access group `$(TeamIdentifierPrefix)com.apple.networkextensionsharing`. The OS uses SecItemCopyMatching(_:_:) to obtain a persistent reference to each certificate from the application’s keychain and uses it during EAP authentication.

The number of elements in the certificate array may not be more than 10.

## See Also

### Setting Keychain-based EAP Properties

func setIdentity(SecIdentity) -> Bool

Sets the client identity for EAP authentication.

