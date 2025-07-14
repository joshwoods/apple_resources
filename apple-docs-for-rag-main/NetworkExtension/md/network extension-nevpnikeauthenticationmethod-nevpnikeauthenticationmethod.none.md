

- Network Extension
- NEVPNIKEAuthenticationMethod
-  NEVPNIKEAuthenticationMethod.none 

Case

# NEVPNIKEAuthenticationMethod.none

Do not authenticate with the IPSec server. Note that extended authentication may still be performed if the useExtendedAuthentication property is set. This value is only valid for IKE version 2 (IKEv2)

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
case none
```

## See Also

### Authentication methods

case certificate

Use a certificate and private key as the authentication credential. The certificate and private key set in the identityReference or identityData property will be used.

case sharedSecret

Use a shared secret as the authentication credential. The shared secret set in the sharedSecretReference property will be used.

