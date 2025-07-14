

- GSS
-  Credential Management 

API Collection

# Credential Management

Securely establish connections between endpoints.

## Topics

### Allocation and Deallocation

func GSSCreateCredentialFromUUID(CFUUID) -> gss_cred_id_t?

Creates a credential from a universally unique identifier.

func gss_add_cred(UnsafeMutablePointer&lt;OM_uint32>, gss_cred_id_t?, gss_name_t?, gss_OID?, gss_cred_usage_t, OM_uint32, OM_uint32, UnsafeMutablePointer&lt;gss_cred_id_t?>, UnsafeMutablePointer&lt;gss_OID_set?>?, UnsafeMutablePointer&lt;OM_uint32>?, UnsafeMutablePointer&lt;OM_uint32>?) -> OM_uint32

Adds a new credential element to an existing credential.

func gss_set_cred_option(UnsafeMutablePointer&lt;OM_uint32>, UnsafeMutablePointer&lt;gss_cred_id_t?>?, gss_OID, gss_buffer_t?) -> OM_uint32

Changes a credential option.

func gss_release_cred(UnsafeMutablePointer&lt;OM_uint32>, UnsafeMutablePointer&lt;gss_cred_id_t?>) -> OM_uint32

Releases the memory of a credential.

func gss_destroy_cred(UnsafeMutablePointer&lt;OM_uint32>, UnsafeMutablePointer&lt;gss_cred_id_t?>) -> OM_uint32

Purges a credential from memory.

### Initial Credential Keys

The keys used in the attributes dictionary when acquiring new credentials.

var kGSSICPassword: String

The value is a string that indicates a password.

var kGSSICCertificate: String

The value that indicates a certificate to use with PKINIT/PKU2U.

var kGSSCredentialUsage: String

The value indicates how to use the credential.

var kGSSICVerifyCredential: String

The value indicates whether to validate the credential with a trusted source to ensure there was no machine-in-the-middle attack.

var kGSSICLKDCHostname: String

The value is a string indicating the LKDC hostname.

var kGSSICKerberosCacheName: String

The value is a string indicating the name of the cache created for use with the Kerberos mechanism.

var kGSSICSiteName: String

The value is a string that is the name of site you are authenticating with, used for load balancing in DNS in Kerberos.

var kGSSICAppIdentifierACL: String

The value is an array of strings containing the list of bundle ID prefixes allowed to access this credential.

var kGSSICCreateNewCredential: String

The value is a Boolean that indicates whether the caller wants to create a new credential and not overwrite a credential with the same name.

var kGSSICAppleSourceApp: String

The value is a dictionary indicating attributes of the app that the credential is for (only applies to AppVPN).

var kGSSICVerifyCredentialAcceptorName: String

The value is a string indicating the name of the acceptor.

var kGSSICAuthenticationContext: String

The value indicates whether to allow the authentication UI or a context to pass a pre-evaluated authentication context.

### Pseudo Random Constants

var GSS_C_PRF_KEY_FULL: Int32

This value indicates using the sub-session key by acceptor, initiator, or the ticket’s session key.

var GSS_C_PRF_KEY_PARTIAL: Int32

This value indicates using the sub-session key the initiator or the ticket’s session key.

### Credential Usage Values

The values for use with the credential usage key.

var kGSS_C_INITIATE: String

The value that indicates a credential may be used to initiate a context.

var kGSS_C_ACCEPT: String

The value that indicates that a credential may be used to accept a context.

var kGSS_C_BOTH: String

The value that indicates that a credential may be used to either initiate or accept a context.

### Password Keys

The keys used in the attributes dictionary for the changing passwords.

var kGSSChangePasswordOldPassword: String

The value is a string that indicates the old password.

var kGSSChangePasswordNewPassword: String

The value is a string that indicates the new password.

### Credential Masks and Macros

var GSS_C_INDEFINITE: UInt

The value that indicates the maximum permitted lifetime when used in a time request.

var GSS_C_INITIATE: Int32

The value that indicates a credential that can initiate a security context.

var GSS_C_ACCEPT: Int32

The value that indicates a credential that can accept a security context.

var GSS_C_BOTH: Int32

The value that indicates a credential that can both initiate and accept security contexts.

var GSS_C_OPTION_MASK: Int32

The masking constant for options.

var GSS_C_CRED_NO_UI: Int32

The value that indicates no UI.

typealias gss_auth_identity_t

A pointer to an opaque object used to manage authentication identities.

typealias gss_const_cred_id_t

A pointer to an immutable opaque type that you use to exchange a credential object with GSS-API functions.

typealias gss_cred_id_t

A pointer to an opaque type that you use to exchange a credential object with GSS-API functions.

typealias gss_cred_usage_t

A credential usage value.

### Acquisition

func gss_aapl_initial_cred(gss_name_t, gss_const_OID, CFDictionary?, UnsafeMutablePointer&lt;gss_cred_id_t?>, UnsafeMutablePointer&lt;Unmanaged&lt;CFError>?>?) -> OM_uint32

Acquires a new credential using a password or certificate.

func gss_acquire_cred(UnsafeMutablePointer&lt;OM_uint32>, gss_name_t?, OM_uint32, gss_OID_set?, gss_cred_usage_t, UnsafeMutablePointer&lt;gss_cred_id_t?>, UnsafeMutablePointer&lt;gss_OID_set?>?, UnsafeMutablePointer&lt;OM_uint32>?) -> OM_uint32

Acquires a credential for use in establishing a security context.

func gss_acquire_cred_with_password(UnsafeMutablePointer&lt;OM_uint32>, gss_name_t, gss_buffer_t, OM_uint32, gss_OID_set?, gss_cred_usage_t, UnsafeMutablePointer&lt;gss_cred_id_t?>, UnsafeMutablePointer&lt;gss_OID_set?>?, UnsafeMutablePointer&lt;OM_uint32>?) -> OM_uint32

Acquires a credential for use in establishing a security context using a password.

func GSSCredentialCopyUUID(gss_cred_id_t) -> Unmanaged&lt;CFUUID>?

Returns a copy of the universally unique identifier corresponding to a GSS credential.

func GSSCredentialCopyName(gss_cred_id_t) -> gss_name_t?

Returns the name describing the credential.

func gss_pseudo_random(UnsafeMutablePointer&lt;OM_uint32>, gss_ctx_id_t, Int32, gss_buffer_t, Int, gss_buffer_t) -> OM_uint32

Returns a pseudo-random byte stream for keying.

### Inquiries

func gss_inquire_cred(UnsafeMutablePointer&lt;OM_uint32>, gss_cred_id_t?, UnsafeMutablePointer&lt;gss_name_t?>?, UnsafeMutablePointer&lt;OM_uint32>?, UnsafeMutablePointer&lt;gss_cred_usage_t>?, UnsafeMutablePointer&lt;gss_OID_set?>?) -> OM_uint32

Obtains information about a credential.

func gss_inquire_cred_by_mech(UnsafeMutablePointer&lt;OM_uint32>, gss_cred_id_t?, gss_OID, UnsafeMutablePointer&lt;gss_name_t?>?, UnsafeMutablePointer&lt;OM_uint32>?, UnsafeMutablePointer&lt;OM_uint32>?, UnsafeMutablePointer&lt;gss_cred_usage_t>?) -> OM_uint32

Obtains per-mechanism information about a credential.

func gss_inquire_cred_by_oid(UnsafeMutablePointer&lt;OM_uint32>, gss_cred_id_t, gss_OID, UnsafeMutablePointer&lt;gss_buffer_set_t?>) -> OM_uint32

Inquires about a particular characteristic of a credential.

func GSSCredentialGetLifetime(gss_cred_id_t) -> OM_uint32

Returns the remaining time in seconds before the credential expires.

### Iteration

func gss_iter_creds(UnsafeMutablePointer&lt;OM_uint32>, OM_uint32, gss_const_OID?, (gss_OID?, gss_cred_id_t?) -> Void) -> OM_uint32

Iterates over all credentials.

func gss_iter_creds_f(UnsafeMutablePointer&lt;OM_uint32>, OM_uint32, gss_const_OID?, UnsafeMutableRawPointer?, (UnsafeMutableRawPointer?, gss_OID?, gss_cred_id_t?) -> Void) -> OM_uint32

Iterates over all credentials with a user context.

### Import and Export

func gss_import_cred(UnsafeMutablePointer&lt;OM_uint32>, gss_buffer_t, UnsafeMutablePointer&lt;gss_cred_id_t?>) -> OM_uint32

Imports a credential from a token.

func gss_export_cred(UnsafeMutablePointer&lt;OM_uint32>, gss_cred_id_t, gss_buffer_t) -> OM_uint32

Exports a credential to a token.

## See Also

### Credentials

Security Mechanisms

Provide a security mechanism for your implementation.

