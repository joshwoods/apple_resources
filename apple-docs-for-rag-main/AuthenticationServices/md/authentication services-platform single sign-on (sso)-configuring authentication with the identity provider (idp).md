

- Authentication Services
- Platform single sign-on (SSO)
-  Configuring authentication with the identity provider (IdP) 

Article

# Configuring authentication with the identity provider (IdP)

Specify how platform SSO authenticates with the identity provider.

## Overview

Use a login configuration to instruct platform SSO how to authenticate with the identity provider.

Use additionalAuthorizationScopes to differentiate authentication requests for network account authorization from other login requests. For example, these requests can return temporary admin group membership.

The accountDisplayName is the user-friendly name for the IdP, and replaces “identity provider” in notifications and the authentication dialog.

### Configure for federation

Federation enables authentication between security domains, such as from a local IdP to a cloud IdP. You have two options to configure platform SSO for federation:

WS-Trust  
Use when federation for the user won’t change.

Dynamic WS-Trust  
Use when federation for the user can change.

To use WS-Trust, set federationType to ASAuthorizationProviderExtensionLoginConfiguration.FederationType.wsTrust. This federation type sends the WS-Trust request to the URLs in the metadata exchange data (MEX) response. The required configuration values are:

federationMEXURL  
The MEX URL for federation.

federationRequestURN  
The URN for the WS-Trust login request.

To use Dynamic WS-Trust, set federationType to ASAuthorizationProviderExtensionLoginConfiguration.FederationType.dynamicWSTrust. Dynamic WS-Trust sends a preauthentication to the IdP to determine whether to use federation and where to authenticate. The required configuration values are:

federationRequestURN  
The URN for the WS-Trust login request.

federationUserPreauthenticationURL  
The URL for the pre-authentication request.

federationPredicate  
The predicate to evaluate the pre-authentication response. If it evaluates to true, then the authentication proceeds with WS-Trust. If false, the system uses normal password authentication.

federationMEXURLKeypath  
The key path in the pre-authentication response for the MEX URL, for use only if the `federationPredicate` evaluates to true.

### Use the login manager to interface with Platform SSO

The SSO extension uses ASAuthorizationProviderExtensionLoginManager to interface with platform SSO. The system provides and instance of the login manager for each authentication request. The login manager can:

- Update the login configuration.

- Update SSO tokens.

- Request that the user authenticate again in the case of expired credentials.

- Access the device keys to sign, encrypt, and decrypt additional requests.

- Restart registration if an unrecoverable error occurs.

If the extension detects that the keys or the device become compromised due to a security exploit, it can reset the keys and request device registration again. In this case, the extension needs to return `failedNoRetry` during registration until macOS is patched.

### Migrate from per-user device keys to shared device keys

Devices keys represent the device to the IdP. They keys can either be *per-user*, which means each user on the device has separate keys, or *shared*, which means all users on the device use the same keys. Shared device keys enable a device to authenticate with the IdP before a user logs in. Shared keys are available in macOS 14 and later.

The following table summarizes feature availability for per-user device keys and shared device keys:

| Feature | Per-User Device Keys | Shared Device Keys |
|----|----|----|
| *Authentication* |  |  |
| Password | ✓ | ✓ |
| User Secure Enclave key | ✓ | ✓ |
| SmartCard | ✓ | ✓ |
| *Create user* |  |  |
| Password |  | ✓ |
| SmartCard |  | ✓ |
| *Unlock with IdP credentials* |  |  |
| Login window |  | ✓ (platform SSO 2.0 only) |
| Screensaver unlock |  | ✓ (platform SSO 2.0 only) |
| *Other* |  |  |
| Group membership | ✓ | ✓ |
| Network account authorization |  | ✓ |

To migrate from user keys to shared keys you need to create new secure enclave backed keys and register these with the server. To facilitate this, the system initiates device registration on the SSO extension for migration with the registrationDeviceKeyMigration option set. Both the user keys and the new shared keys are available only during this call. Use key(for:) to access them. The SSO extension needs to register the new shared keys with the server and can use the existing user keys to provide a chain of trust.

When Device registration completes successfully, the system initiates user registration with the registrationDeviceKeyMigration option set. You also need to migrate any user-specific login configuration to the ASAuthorizationProviderExtensionUserLoginConfiguration at this time. When user registration completes successfully, the system destroys the user keys and previous login configuration. For subsequent users, the same user registration flow repeats and the system destroys the user keys after a successful response.

## See Also

### Configuration

Configuring Device Management

Configure Device Management to support device and user registration for platform SSO.

class ASAuthorizationProviderExtensionLoginConfiguration

An interface for configuring platform single sign-on.

class ASAuthorizationProviderExtensionLoginManager

An interface to maintain platform single sign-on (SSO) during authentication and registration.

