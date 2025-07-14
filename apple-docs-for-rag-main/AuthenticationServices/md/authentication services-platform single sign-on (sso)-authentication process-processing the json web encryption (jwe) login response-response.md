

- Authentication Services
- Platform single sign-on (SSO)
- Authentication process
-  Processing the JSON Web Encryption (JWE) login response 

Article

# Processing the JSON Web Encryption (JWE) login response

Validate the encrypted response.

## Overview

Your login configuration instructs platform SSO how to receive and verify the login response from an identity provider (IdP).

If the HTTP response code is `200`, the system decrypts the response body according to RFC 7516 Section 5.2, using JWE Compact Serialization. Use of the zip header isn’t supported. The system checks `PartyUInfo` for the Ephemeral Public Key in the response. `PartyVInfo` is the `jwe_crypto.apv` from the login request.

The following code sample provides an example of an encrypted login response JWE:

```
HTTP/1.1 200 OK
Cache-Control: no-store, no-cache
Pragma: no-cache
Content-Type: application/platformsso-login-response+jwt; charset=utf-8
ewogI...luEng
```

For more information, see Creating a JSON Web Encryption (JWE) login response.

### Validate the ID token

The `id_token` is a JSON Object Signing and Encryption (JOSE) object that the IdP signs using either RS256 or ES256 algorithms per RFC 7515 using compact serialization. The system retrieves the signing keys from the jwksEndpointURL.

The following table specifies the values that the system uses to validate the ID token:

| Key | Value | Notes |
|----|----|----|
| `nonce` | The `nonce` value from the login request. | Required. |
| `iss` | Must match the issuer. | Required. |
| `aud` | Must match the clientID or must contain the clientID. | Required. |
| `azp` | If present, must match the clientID. | Required only if `aud` is an array. |
| `iat` | Must be in past. | Required. |
| `exp` | Must be in the future. | Required. |
| `nbf` | If present, must be in the past. | Optional. |
| `groups` or groupResponseClaimName | The requested group membership for the user. | Optional. |

If validation succeeds, the system saves the response tokens to the keychain using the keychain data-protection attribute kSecAttrAccessibleAfterFirstUnlockThisDeviceOnly and checks the Kerberos mapping.

For a group membership request, the system adds the user to the groups that the IdP supplies in the `id_token`, and it removes the user from the groups not returned. The system ignores groups that you didn’t specify in the Device Management profile.

For more information, see Configuring Device Management.

## See Also

### Login response

Creating a JSON Web Encryption (JWE) login response

Create an encrypted login response and configure the concatenation key derivation function (Concat KDF).

Performing encryption verification

Verify the login request and create a JSON Web Encryption (JWE) response.

