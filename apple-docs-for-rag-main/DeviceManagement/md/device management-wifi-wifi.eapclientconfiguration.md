

- Device Management
- WiFi
-  WiFi.EAPClientConfiguration 

Device Management Profile

# WiFi.EAPClientConfiguration

A dictionary that configures an enterprise network.

iOS 4.0+iPadOS 4.0+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 3.2+Device Assignment ServicesVPP License Management

``` source
object WiFi.EAPClientConfiguration
```

## Properties

`AcceptEAPTypes`

`[integer]`

 (Required) 

The EAP types that the system accepts. Allowed values:

13  
TLS

Possible Values: `13, 17, 18, 21, 23, 25, 43`

`EAPFASTProvisionPAC`

`boolean`

Default: `false`

`EAPFASTProvisionPACAnonymously`

`boolean`

Default: `false`

`EAPFASTUsePAC`

`boolean`

Default: `false`

`EAPSIMNumberOfRANDs`

`integer`

Default: `3`

Possible Values: `2, 3`

`OneTimeUserPassword`

`boolean`

Default: `false`

`OuterIdentity`

`string`

`PayloadCertificateAnchorUUID`

`[string]`

`SystemModeCredentialsSource`

`string`

`SystemModeUseOpenDirectoryCredentials`

`boolean`

Default: `false`

`TLSAllowTrustExceptions`

`boolean`

Deprecated 

Default: `true`

`TLSCertificateIsRequired`

`boolean`

Default: `false`

`TLSMaximumVersion`

`string`

Default: `1.2`

Possible Values: `1.0, 1.1, 1.2, 1.3`

`TLSMinimumVersion`

`string`

Default: `1.0`

Possible Values: `1.0, 1.1, 1.2, 1.3`

`TLSTrustedCertificates`

`[string]`

`TLSTrustedServerNames`

`[string]`

`TTLSInnerAuthentication`

`string`

Default: `MSCHAPv2`

Possible Values: `PAP, EAP, CHAP, MSCHAP, MSCHAPv2`

`UserName`

`string`

`UserPassword`

`string`

## Overview

17  
LEAP

18  
EAP-SIM

21  
TTLS

23  
EAP-AKA

25  
PEAP

43  
EAP-FAST

For EAP-TLS authentication without a network payload, install the necessary identity certificates and have your users select EAP-TLS mode in the 802.1X credentials dialog that appears when they connect to the network. For other EAP types, a network payload is necessary and must specify the correct settings for the network.

- EAPFASTProvisionPAC: If `true`, allows PAC provisioning.

  This value is only applicable if `EAPFASTUsePAC` is `true`. This value must be `true` for EAP-FAST PAC usage to succeed because there’s no other way to provision a PAC.

- EAPFASTProvisionPACAnonymously: If `true`, provisions the device anonymously. Note that there are known machine-in-the-middle attacks for anonymous provisioning.

- EAPFASTUsePAC: If `true`, the device uses an existing PAC if it’s present. Otherwise, the server must present its identity using a certificate.

- EAPSIMNumberOfRANDs: The minimum number of RAND values to accept from the server.

  For use with EAP-SIM only.

- OneTimeUserPassword: If `true`, the user receives a prompt for a password each time they connect to the network.

- OuterIdentity: A name that hides the user’s true name. The user’s actual name appears only inside the encrypted tunnel. For example, you might set this to *anonymous* or *anon*, or *anon@mycompany.net*. It can increase security because an attacker can’t see the authenticating user’s name in the clear.

  This key is only relevant to TTLS, PEAP, and EAP-FAST.

  This field is required if `TLSMinimumVersion` is `1.3`.

- PayloadCertificateAnchorUUID: An array of the UUID of a certificate payloads in the same profile to trust for authentication. Use this key to prevent the device from asking the user whether to trust the listed certificates. Dynamic trust (the certificate dialogue) is in a disabled state if you specify this property without also enabling `TLSAllowTrustExceptions`.

- SystemModeCredentialsSource: Set this string to `ActiveDirectory` to use the AD computer name and password credentials.

  If using this property, you can’t use `SystemModeUseOpenDirectoryCredentials`.

- SystemModeUseOpenDirectoryCredentials: If `true`, the system mode connection tries to use the Open Directory credentials.

  If using this property, you can’t use `SystemModeCredentialsSource`.

- TLSAllowTrustExceptions: If `true`, allows a dynamic trust decision by the user. The dynamic trust is the certificate dialogue that appears when the system doesn’t trust a certificate.

  If `false`, the authentication fails if the system doesn’t already trust the certificate.

  As of iOS 8, Apple no longer supports this key.

- TLSCertificateIsRequired: If `true`, allows for two-factor authentication for EAP-TTLS, PEAP, or EAP-FAST. If `false`, allows for zero-factor authentication for EAP-TLS.

  If you don’t specify a value, the default is `true` for EAP-TLS, and `false` for other EAP types.

- TLSMaximumVersion: The maximum TLS version for EAP authentication.

- TLSMinimumVersion: The minimum TLS version for EAP authentication.

- TLSTrustedCertificates: An array of trusted certificates. Each entry in the array must contain certificate data that represents an anchor certificate used for verifying the server certificate.

- TLSTrustedServerNames: The list of accepted server certificate common names. If a server presents a certificate that isn’t in this list, the system doesn’t trust it.

  If you specify this property, the system disables dynamic trust (the certificate dialog) unless you also specify `TLSAllowTrustExceptions` with the value `true`.

  If necessary, use wildcards to specify the name, such as `wpa.*.example.com`.

- TTLSInnerAuthentication: The inner authentication that the TTLS module uses.

- UserName: The user name for the account. If you don’t specify a value, the system prompts the user during login.

- UserPassword: The user’s password. If you don’t specify a value, the system prompts the user during login.

## See Also

### Objects

object WiFi.QoSMarkingPolicy

A dictionary that defines the quality-of-service settings.

