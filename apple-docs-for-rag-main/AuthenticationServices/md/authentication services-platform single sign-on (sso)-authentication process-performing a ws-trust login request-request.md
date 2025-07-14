

- Authentication Services
- Platform single sign-on (SSO)
- Authentication process
-  Performing a WS-Trust login request 

Article

# Performing a WS-Trust login request

Create a WS-Trust login request using the metadata exchange data (MEX) response.

## Overview

After receiving a WS-Trust MEX response, the next step that the system performs for federated authentication with WS-Trust, meaning between security domains, is to send a login request to a federated identity provider (IdP).

The system uses the federationRequestURN and the URLs specified in the MEX response to create the WS-Trust login request, per Web Services Security Username Token Profile Version 1.1.1. The system doesn’t support `PasswordDigest`. The system sends the WS-Trust login using Simple Object Access Protocol (SOAP) to the endpoint in the MEX response.

For more information about federated authentication with WS-Trust, see Authentication process.

### Receive the WS-Trust login response

The system loads the SOAP response as XML and validates it, which includes checking that the nonce is correct and the created and expires dates are current. The system then parses the `TokenType` and uses it to set the correct `grant_type` in the platform SSO login request.

## See Also

### Login request

Creating an embedded assertion

Request an embedded assertion for login types that require a digital signature for authentication.

Creating an encrypted embedded assertion

Request an encrypted embedded assertion for login types that require password encryption.

Creating and validating a login request

Create a signed JOSE login request.

Creating a refresh request

Refresh a non-expired token instead of sending a new login request.

Supporting key requests and key exchange requests

Support the platform SSO 2.0 protocol for encryption and decryption operations.

