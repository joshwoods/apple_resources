

- Authentication Services
-  ASAuthorizationProviderExtensionLoginConfiguration 

Class

# ASAuthorizationProviderExtensionLoginConfiguration

An interface for configuring platform single sign-on.

macOS 13.0+

``` source
class ASAuthorizationProviderExtensionLoginConfiguration
```

## Mentioned in 

Creating extensions that support platform SSO

## Overview

This class provides login configuration information for platform single sign-on.

## Topics

### Creating the configuration

init(clientID: String, issuer: String, tokenEndpointURL: URL, jwksEndpointURL: URL, audience: String?)

Creates a configuration with the required values.

class func configuration(openIDConfigurationURL: URL, clientID: String, issuer: String?, completion: (ASAuthorizationProviderExtensionLoginConfiguration?, (any Error)?) -> Void)

Creates a login configuration using the OpenID configuration.

### Obtaining the required configuration

var audience: String

The audience for validation and requests.

var clientID: String

The identifier for the client at the identity provider.

var jwksEndpointURL: URL

The JSON Web Key Set endpoint URL for keys.

var tokenEndpointURL: URL

The token endpoint URL for login requests.

var issuer: String

The issuer of the identity token that the identity provider returns.

### Obtaining the recommended configuration

var accountDisplayName: String?

The display name for the account.

var invalidCredentialPredicate: String?

The predicate string that identifies invalid credential errors.

### Configuring the server nonce

var customNonceRequestValues: [URLQueryItem]

Custom values to add to the server nonce POST request body.

var nonceEndpointURL: URL

The URL to retrieve a one-time use value from the server.

var nonceResponseKeypath: String

The keypath in the response that contains the one-time use value.

var serverNonceClaimName: String

The name of the claim to include in authentication requests.

### Configuring the previous refresh token

var includePreviousRefreshTokenInLoginRequest: Bool

A Boolean value that indicates whether to include the previous refresh token in the authentation request.

var previousRefreshTokenClaimName: String

The claim name for the previous single sign-on token value in the authentication request.

### Customizing the authentication request

func setCustomAssertionRequestBodyClaims([String : Any]) throws

Adds the custom claims to the embedded assertion request body.

func setCustomAssertionRequestHeaderClaims([String : Any]) throws

Adds the custom claims to the embedded assertion request header.

func setCustomLoginRequestBodyClaims([String : Any]) throws

Adds the custom claims to the login request body.

func setCustomLoginRequestHeaderClaims([String : Any]) throws

Adds the custom claims to the login request header.

var additionalScopes: String

A set of extra scopes to add to the base for the authentication request.

var customLoginRequestValues: [URLQueryItem]

Provider-supplied values to add to the login POST request body.

var kerberosTicketMappings: [ASAuthorizationProviderExtensionKerberosMapping]

The set of ticket mappings the system uses to import Kerberos tickets from the single sign-on token.

### Instance Properties

var additionalAuthorizationScopes: String?

var customFederationUserPreauthenticationRequestValues: [URLQueryItem]

var customKeyExchangeRequestValues: [URLQueryItem]

var customKeyRequestValues: [URLQueryItem]

var customRefreshRequestValues: [URLQueryItem]

var customRequestJWTParameterName: String?

var deviceContext: Data?

var federationMEXURL: URL?

var federationMEXURLKeypath: String?

var federationPredicate: String?

var federationRequestURN: String?

var federationType: ASAuthorizationProviderExtensionLoginConfiguration.FederationType

var federationUserPreauthenticationURL: URL?

var groupRequestClaimName: String?

var groupResponseClaimName: String?

var jwksTrustedRootCertificates: [SecCertificate]

var keyEndpointURL: URL?

var loginRequestEncryptionAPVPrefix: Data?

var loginRequestEncryptionPublicKey: SecKey?

var refreshEndpointURL: URL?

var uniqueIdentifierClaimName: String?

var userSecureEnclaveKeyBiometricPolicy: ASAuthorizationProviderExtensionLoginConfiguration.UserSecureEnclaveKeyBiometricPolicy

var hpkeAuthPublicKey: SecKey?

var hpkePreSharedKey: Data?

var hpkePreSharedKeyID: Data?

var loginRequestEncryptionAlgorithm: ASAuthorizationProviderExtensionEncryptionAlgorithm

var loginRequestHPKEPreSharedKey: Data?

var loginRequestHPKEPreSharedKeyID: Data?

### Instance Methods

func setCustomKeyExchangeRequestBodyClaims([String : Any]) throws

func setCustomKeyExchangeRequestHeaderClaims([String : Any]) throws

func setCustomKeyRequestBodyClaims([String : Any]) throws

func setCustomKeyRequestHeaderClaims([String : Any]) throws

func setCustomRefreshRequestBodyClaims([String : Any]) throws

func setCustomRefreshRequestHeaderClaims([String : Any]) throws

### Structures

struct UserSecureEnclaveKeyBiometricPolicy

### Enumerations

enum FederationType

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Configuration

Configuring Device Management

Configure Device Management to support device and user registration for platform SSO.

Configuring authentication with the identity provider (IdP)

Specify how platform SSO authenticates with the identity provider.

class ASAuthorizationProviderExtensionLoginManager

An interface to maintain platform single sign-on (SSO) during authentication and registration.

