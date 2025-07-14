

- Open Directory
- OpenDirectory Functions
-  Authentication Types 

API Collection

# Authentication Types

Types of authentication available in Open Directory.

## Topics

### Constants

let kODAuthenticationType2WayRandom: String

The authentication type used to specify two way random authentication.

let kODAuthenticationType2WayRandomChangePasswd: String

The authentication type used to change a user’s password using two way random authentication.

let kODAuthenticationTypeAPOP: String

The authentication type used to specify APOP authentication.

let kODAuthenticationTypeCRAM_MD5: String

The authentication type used to specify CRAM MD5 authentication.

let kODAuthenticationTypeChangePasswd: String

The authentication type used to change a user’s password using CRAM MD5 authentication.

let kODAuthenticationTypeClearText: String

The authentication type used to specify cleartext authentication.

let kODAuthenticationTypeCrypt: String

The authentication type used to specify crypt authentication, which uses a crypt password stored in a user’s record if available.

let kODAuthenticationTypeDIGEST_MD5: String

The authentication type used to specify digest MD5 authentication.

let kODAuthenticationTypeDeleteUser: String

The authentication type used to specify that a user on an Apple password server be deleted.

let kODAuthenticationTypeGetEffectivePolicy: String

The authentication type used to access the policies applied to a user.

let kODAuthenticationTypeGetGlobalPolicy: String

The authentication type used to access the global authentication policy.

let kODAuthenticationTypeGetKerberosPrincipal: String

The authentication type used to access the name of the Kerberos principal.

let kODAuthenticationTypeGetPolicy: String

The authentication type used to specify that the plug-in should determine the authentication method to use.

let kODAuthenticationTypeGetUserData: String

The authentication type used to access user data on an Apple password server.

let kODAuthenticationTypeGetUserName: String

The authentication type used to access a username on an Apple password server.

let kODAuthenticationTypeKerberosTickets: String

The authentication type used to provide write access to LDAP with an existing Kerberos ticket.

let kODAuthenticationTypeMPPEMasterKeys: String

The authentication type used to specify primary keys for MPPE encryption.

let kODAuthenticationTypeMSCHAP2: String

The authentication type used to specify MS-CHAPv2 encryption.

let kODAuthenticationTypeNTLMv2: String

The authentication type used to verify an NTLMv2 challenge and response.

let kODAuthenticationTypeNTLMv2WithSessionKey: String

The authentication type used to verify an NTLMv2 challenge and response and retrieve session keys in a single call.

let kODAuthenticationTypeNewUser: String

The authentication type used to create a new user on an Apple password server.

let kODAuthenticationTypeNewUserWithPolicy: String

The authentication type used to create a new user with specified policy settings on an Apple password server.

let kODAuthenticationTypeNodeNativeClearTextOK: String

The authentication type used to specify that the plug-in should determine the authentication method to use. It also specifies that cleartext is an acceptable authentication method.

let kODAuthenticationTypeNodeNativeNoClearText: String

The authentication type used to specify that the plug-in should determine the authentication method to use. It also specifies that cleartext is not an acceptable authentication method.

let kODAuthenticationTypeReadSecureHash: String

The authentication type used to access the SHA1 or seeded SHA1 hash for a local user.

let kODAuthenticationTypeSMBNTv2UserSessionKey: String

The authentication type used to generate an NTLMv2 user session key.

let kODAuthenticationTypeSMBWorkstationCredentialSessionKey: String

The authentication type used to generate an SMB workstation credential session key.

let kODAuthenticationTypeSMB_LM_Key: String

The authentication type used to specify SMB LAN manager authentication.

let kODAuthenticationTypeSMB_NT_Key: String

The authentication type used to specify SMB NT authentication.

let kODAuthenticationTypeSMB_NT_UserSessionKey: String

The authentication type used by Samba to access session keys on an Apple password server.

let kODAuthenticationTypeSMB_NT_WithUserSessionKey: String

The authentication type used by Samba to authenticate and access session keys on an Apple password server.

let kODAuthenticationTypeSetGlobalPolicy: String

The authentication type used to set the global authentication policy.

let kODAuthenticationTypeSetLMHash: String

The authentication type used to set the LAN manager hash for an account.

let kODAuthenticationTypeSetNTHash: String

The authentication type used to set the NT hash for a user.

let kODAuthenticationTypeSetPassword: String

The authentication type used to set a password.

let kODAuthenticationTypeSetPasswordAsCurrent: String

The authentication type used to set a password using the current credentials.

let kODAuthenticationTypeSetPolicy: String

The authentication type used to specify that the plug-in should determine the authentication method to use.

let kODAuthenticationTypeSetPolicyAsCurrent: String

The authentication type used to set the authentication policy using the current credentials.

let kODAuthenticationTypeSetUserData: String

The authentication type used to set user data on an Apple password server.

let kODAuthenticationTypeSetUserName: String

The authentication type used to set a username on an Apple password server.

let kODAuthenticationTypeSetWorkstationPassword: String

An authentication type used to support PDC SMB interaction with Directory Services.

let kODAuthenticationTypeWithAuthorizationRef: String

The authentication type used to allow root access to local directories with valid authorization.

let kODAuthenticationTypeWriteSecureHash: String

The authentication type used to enable a root process to write the secure hash of a user record.

let kODAuthenticationTypeSetCertificateHashAsCurrent: String

An authentication type to set the certificate using the authenticated user’s credentials.

## See Also

### Constants

Session Keys

Keys used when specifying session information.

Node Types

Open Directory node types.

Match Types

Types of matches used for searches.

Record Types

Types of Open Directory records.

General Attribute Types

Types of Open Directory attributes.

Configuration Attribute Types

Types of Open Directory attributes specifically for use with configure nodes.

