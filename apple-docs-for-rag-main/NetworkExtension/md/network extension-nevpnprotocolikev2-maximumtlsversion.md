

- Network Extension
- NEVPNProtocolIKEv2
-  maximumTLSVersion 

Instance Property

# maximumTLSVersion

The minimum TLS version to allow for EAP-TLS authentication.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 17.0+visionOS 1.0+

``` source
var maximumTLSVersion: NEVPNIKEv2TLSVersion { get set }
```

## Discussion

The default value of this property is NEVPNIKEv2TLSVersion.versionDefault.

## See Also

### Accessing TLS version properties

var minimumTLSVersion: NEVPNIKEv2TLSVersion

The minimum TLS version to allow for EAP-TLS authentication.

enum NEVPNIKEv2TLSVersion

An enumeration of TLS Versions for use in EAP-TLS.

