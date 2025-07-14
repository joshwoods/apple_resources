

- Authentication Services
- Platform single sign-on (SSO)
-  Creating extensions that support platform SSO 

Article

# Creating extensions that support platform SSO

Configure capabilities and authentication options for extensions.

## Overview

To perform single sign-on (SSO) with an identity provider (IdP), you need to create an SSO extension that supports platform SSO and implements the required functionality. You also need to indicate the grant types that the extension and IdP support. Optionally, you can include support for platform SSO 2.0, and enable use of the Kerberos SSO extension with the platform SSO ticket-granting ticket (TGT).

The extension completes the necessary actions to register devices and users and perform authentication with an IdP. The IdP server handles the login requests and responses to complete the authentication process. During development, you can run commands in Terminal to view messages from the IdP while you iterate on the configuration.

### Specify supported grant types

The SSO extension you create needs to indicate the grant types that it and the IdP support. In macOS 14.0 and later, implement supportedGrantTypes() and return:

- Password: password

- Secure enclave key, SmartCard, and encrypted password: jwtBearer

- WS-Trust: saml1_1 or saml2_0

If you build your extension with an SDK for macOS 14 or later, the default authentication messages require updates to adhere to the RFC standard. This includes different JSON Web Token (JWT) type headers and parameter names. You can override these values in the ASAuthorizationProviderExtensionLoginConfiguration.

### Implement platform SSO 2.0 capabilities

Platform SSO 2.0 adds a new key service for SSO extensions and IdPs which enables an alternative registration flow and additional login configuration. You need to implement protocolVersion() in the extension and return ASAuthorizationProviderExtensionPlatformSSOProtocolVersion.version2_0 to indicate that the extension and the IdP server support platform SSO 2.0 before using it. You also need to set the keyEndpointURL in the ASAuthorizationProviderExtensionLoginConfiguration.

The key service registers encryption keys to unlock the Mac at the login window and screensaver unlock. There are two kinds of requests: create a key and perform Diffie-Hellman key exchange. The system sends the request to create the key after the user registration call to the SSO extension completes successfully. Then, it binds the key to the user’s account, which involves multiple key exchange requests during this process. The system can only use the key service with shared device keys because it uses the key to unlock the user’s key bag. For more information, see Supporting key requests and key exchange requests.

### Enable ticket-granting ticket (TGT) with the Kerberos SSO extension

Set the following values in the ExtensibleSingleSignOnKerberos.ExtensionData to enable use of the platform SSO TGT with the Kerberos SSO extension:

`usePlatformSSOTGT`  
If true, the Kerberos SSO extension uses the TGT from platform SSO with the same realm. The default is false.

`allowPlatformSSOAuthFallback`  
If true, the user can continue to sign in to the Kerberos SSO extension when using the TGT from platform SSO. The default is true.

`performKerberosOnly`  
If true, the Kerberos SSO extension doesn’t perform password expiration checks, external password change checks, or retrieve the user’s home directory. The default is false.

### Use diagnostics to iterate on the configuration during development

When you’re developing for platform SSO, the IdP can generate sample messages that use the current configuration. Perform these actions in Terminal to check the configuration and state of the SSO tokens while you iterate on the configuration:

View messages  
Run `app-sso platform --messages`. These messages don’t use the real keys for the device and instead use a key generated for each call. The private key is also included to enable compatibility testing with other systems such as the server.

Check the configuration and see the state of the SSO tokens  
Run `app-sso platform --state`.

See high-level requests and results  
Filter the log on subsystem `com.apple.AppSSO` and category `PODiagnostics`.

## See Also

### Essentials

Registering devices and users

Implement device and user registration.

protocol ASAuthorizationProviderExtensionRegistrationHandler

An interface through which a single sign-on (SSO) authentication provider extension registers users and devices for platform SSO.

enum ASAuthorizationProviderExtensionAuthenticationMethod

The platform single sign-on method for the user.

struct ASAuthorizationProviderExtensionRequestOptions

The options for the extension to obtain the status of the registration.

enum ASAuthorizationProviderExtensionRegistrationResult

The registration result.

