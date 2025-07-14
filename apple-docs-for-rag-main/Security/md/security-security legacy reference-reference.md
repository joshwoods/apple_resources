

- Security
-  Security legacy reference 

API Collection

# Security legacy reference

Learn about legacy APIs.

## Topics

### Module directory service

var MDS_CDSAATTR_ACLSUBJECTTYPES: Int32

var MDS_CDSAATTR_ALG_TYPE: Int32

var MDS_CDSAATTR_ATTRIBUTE_TYPE: Int32

var MDS_CDSAATTR_ATTRIBUTE_VALUE: Int32

var MDS_CDSAATTR_AUTHORITY_REQUEST_TYPE: Int32

var MDS_CDSAATTR_AUTHTAGS: Int32

var MDS_CDSAATTR_BUNDLE_TYPEFORMAT: Int32

var MDS_CDSAATTR_CDSAVERSION: Int32

var MDS_CDSAATTR_CERT_CLASSNAME: Int32

var MDS_CDSAATTR_CERT_FIELDNAMES: Int32

var MDS_CDSAATTR_CERT_TYPEFORMAT: Int32

var MDS_CDSAATTR_CONJUNCTIVE_OPS: Int32

var MDS_CDSAATTR_CONTEXT_TYPE: Int32

var MDS_CDSAATTR_CRL_TYPEFORMAT: Int32

var MDS_CDSAATTR_CSP_CUSTOMFLAGS: Int32

var MDS_CDSAATTR_CSP_FLAGS: Int32

var MDS_CDSAATTR_CSP_TYPE: Int32

var MDS_CDSAATTR_DEFAULT_TEMPLATE_TYPE: Int32

var MDS_CDSAATTR_DESC: Int32

var MDS_CDSAATTR_DL_TYPE: Int32

var MDS_CDSAATTR_DYNAMIC_FLAG: Int32

var MDS_CDSAATTR_EMMSPECVERSION: Int32

var MDS_CDSAATTR_EMM_TYPE: Int32

var MDS_CDSAATTR_EMM_VENDOR: Int32

var MDS_CDSAATTR_EMM_VERSION: Int32

var MDS_CDSAATTR_GROUP_ID: Int32

var MDS_CDSAATTR_INTERFACE_GUID: Int32

var MDS_CDSAATTR_MANIFEST: Int32

var MDS_CDSAATTR_MODULE_ID: Int32

var MDS_CDSAATTR_MODULE_NAME: Int32

var MDS_CDSAATTR_MULTITHREAD_FLAG: Int32

var MDS_CDSAATTR_NATIVE_SERVICES: Int32

var MDS_CDSAATTR_OID: Int32

var MDS_CDSAATTR_PATH: Int32

var MDS_CDSAATTR_POLICY_STMT: Int32

var MDS_CDSAATTR_PRODUCT_CUSTOMFLAGS: Int32

var MDS_CDSAATTR_PRODUCT_DESC: Int32

var MDS_CDSAATTR_PRODUCT_FLAGS: Int32

var MDS_CDSAATTR_PRODUCT_VENDOR: Int32

var MDS_CDSAATTR_PRODUCT_VERSION: Int32

var MDS_CDSAATTR_PROTOCOL: Int32

var MDS_CDSAATTR_QUERY_LIMITS: Int32

var MDS_CDSAATTR_READER_CUSTOMFLAGS: Int32

var MDS_CDSAATTR_READER_DESC: Int32

var MDS_CDSAATTR_READER_FLAGS: Int32

var MDS_CDSAATTR_READER_FWVERSION: Int32

var MDS_CDSAATTR_READER_SERIALNUMBER: Int32

var MDS_CDSAATTR_READER_VENDOR: Int32

var MDS_CDSAATTR_READER_VERSION: Int32

var MDS_CDSAATTR_RELATIONAL_OPS: Int32

var MDS_CDSAATTR_REQCREDENTIALS: Int32

var MDS_CDSAATTR_RETRIEVALMODE: Int32

var MDS_CDSAATTR_ROOTCERT: Int32

var MDS_CDSAATTR_ROOTCERT_TYPEFORMAT: Int32

var MDS_CDSAATTR_SAMPLETYPES: Int32

var MDS_CDSAATTR_SC_CUSTOMFLAGS: Int32

var MDS_CDSAATTR_SC_DESC: Int32

var MDS_CDSAATTR_SC_FLAGS: Int32

var MDS_CDSAATTR_SC_FWVERSION: Int32

var MDS_CDSAATTR_SC_SERIALNUMBER: Int32

var MDS_CDSAATTR_SC_VENDOR: Int32

var MDS_CDSAATTR_SC_VERSION: Int32

var MDS_CDSAATTR_SERVICE_MASK: Int32

var MDS_CDSAATTR_SERVICE_TYPE: Int32

var MDS_CDSAATTR_SSID: Int32

var MDS_CDSAATTR_STANDARD_DESC: Int32

var MDS_CDSAATTR_STANDARD_VERSION: Int32

var MDS_CDSAATTR_TEMPLATE_FIELD_NAMES: Int32

var MDS_CDSAATTR_USEETAG: Int32

var MDS_CDSAATTR_USEE_TAGS: Int32

var MDS_CDSAATTR_VALUE: Int32

var MDS_CDSAATTR_VENDOR: Int32

var MDS_CDSAATTR_XLATIONTYPEFORMAT: Int32

var MDS_CDSADIR_AC_PRIMARY_NUM_ATTRIBUTES: Int32

var MDS_CDSADIR_CL_ENCAPSULATED_PRODUCT_NUM_ATTRIBUTES: Int32

var MDS_CDSADIR_CL_PRIMARY_NUM_ATTRIBUTES: Int32

var MDS_CDSADIR_COMMON_NUM_ATTRIBUTES: Int32

var MDS_CDSADIR_CSP_CAPABILITY_NUM_ATTRIBUTES: Int32

var MDS_CDSADIR_CSP_ENCAPSULATED_PRODUCT_NUM_ATTRIBUTES: Int32

var MDS_CDSADIR_CSP_PRIMARY_NUM_ATTRIBUTES: Int32

var MDS_CDSADIR_CSP_SC_INFO_NUM_ATTRIBUTES: Int32

var MDS_CDSADIR_CSSM_NUM_ATTRIBUTES: Int32

var MDS_CDSADIR_DL_ENCAPSULATED_PRODUCT_NUM_ATTRIBUTES: Int32

var MDS_CDSADIR_DL_PRIMARY_NUM_ATTRIBUTES: Int32

var MDS_CDSADIR_EMM_NUM_ATTRIBUTES: Int32

var MDS_CDSADIR_EMM_PRIMARY_NUM_ATTRIBUTES: Int32

var MDS_CDSADIR_NUM_RELATIONS: Int32

var MDS_CDSADIR_SCHEMA_ATTRIBUTES_NUM_ATTRIBUTES: Int32

var MDS_CDSADIR_SCHEMA_INDEXES_NUM_ATTRIBUTES: Int32

var MDS_CDSADIR_SCHEMA_RELATONS_NUM_ATTRIBUTES: Int32

var MDS_CDSADIR_TP_ENCAPSULATED_PRODUCT_NUM_ATTRIBUTES: Int32

var MDS_CDSADIR_TP_OIDS_NUM_ATTRIBUTES: Int32

var MDS_CDSADIR_TP_PRIMARY_NUM_ATTRIBUTES: Int32

var MDS_CDSA_DIRECTORY_NAME: String

var MDS_CDSA_SCHEMA_START: Int32

var MDS_OBJECT_DIRECTORY_NAME: String

var MDS_OBJECT_NUM_ATTRIBUTES: Int32

var MDS_OBJECT_NUM_RELATIONS: Int32

var MDS_OBJECT_RECORDTYPE: Int32

typealias MDS_HANDLE

### Protocols

protocol OS_sec_certificate

protocol OS_sec_identity

protocol OS_sec_object

A `sec_object` is a generic, ARC-able type wrapper for common CoreFoundation Security types.

protocol OS_sec_protocol_metadata

A `sec_protocol_metadata` instance conatins read-only properties of a connected and configured security protocol. Clients use this object to read information about a protocol instance. Properties include, for example, the negotiated TLS version, ciphersuite, and peer certificates.

protocol OS_sec_protocol_options

A `sec_protocol_options` instance is a container of options for security protocol instances, such as TLS. Protocol options are used to configure security protocols in the network stack. For example, clients may set the maximum and minimum allowed TLS versions through protocol options.

protocol OS_sec_trust

These are os_object compatible and ARC-able wrappers around existing CoreFoundation Security types, including: SecTrustRef, SecIdentityRef, and SecCertificateRef. They allow clients to use these types in os_object-type APIs and data structures. The underlying CoreFoundation types may be extracted and used by clients as needed.

### Variables

let gGuidAppleCSP: cssm_guid

let gGuidAppleCSPDL: cssm_guid

let gGuidAppleDotMacDL: cssm_guid

let gGuidAppleDotMacTP: cssm_guid

let gGuidAppleFileDL: cssm_guid

let gGuidAppleLDAPDL: cssm_guid

let gGuidAppleSdCSPDL: cssm_guid

let gGuidAppleX509CL: cssm_guid

let gGuidAppleX509TP: cssm_guid

let gGuidCssm: cssm_guid

### Functions

func sec_certificate_copy_ref(sec_certificate_t) -> Unmanaged&lt;SecCertificate>

func sec_certificate_create(SecCertificate) -> sec_certificate_t?

func sec_identity_access_certificates(sec_identity_t, (sec_certificate_t) -> Void) -> Bool

func sec_identity_copy_certificates_ref(sec_identity_t) -> Unmanaged&lt;CFArray>?

func sec_identity_copy_ref(sec_identity_t) -> Unmanaged&lt;SecIdentity>?

func sec_identity_create(SecIdentity) -> sec_identity_t?

func sec_identity_create_with_certificates(SecIdentity, CFArray) -> sec_identity_t?

func sec_protocol_metadata_access_distinguished_names(sec_protocol_metadata_t, (dispatch_data_t) -> Void) -> Bool

func sec_protocol_metadata_access_ocsp_response(sec_protocol_metadata_t, (dispatch_data_t) -> Void) -> Bool

func sec_protocol_metadata_access_peer_certificate_chain(sec_protocol_metadata_t, (sec_certificate_t) -> Void) -> Bool

func sec_protocol_metadata_access_pre_shared_keys(sec_protocol_metadata_t, (dispatch_data_t, dispatch_data_t) -> Void) -> Bool

func sec_protocol_metadata_access_supported_signature_algorithms(sec_protocol_metadata_t, (UInt16) -> Void) -> Bool

func sec_protocol_metadata_challenge_parameters_are_equal(sec_protocol_metadata_t, sec_protocol_metadata_t) -> Bool

func sec_protocol_metadata_copy_peer_public_key(sec_protocol_metadata_t) -> dispatch_data_t?

func sec_protocol_metadata_create_secret(sec_protocol_metadata_t, Int, UnsafePointer&lt;CChar>, Int) -> dispatch_data_t?

func sec_protocol_metadata_create_secret_with_context(sec_protocol_metadata_t, Int, UnsafePointer&lt;CChar>, Int, UnsafePointer&lt;UInt8>, Int) -> dispatch_data_t?

func sec_protocol_metadata_get_early_data_accepted(sec_protocol_metadata_t) -> Bool

func sec_protocol_metadata_get_negotiated_ciphersuite(sec_protocol_metadata_t) -> SSLCipherSuiteDeprecated

func sec_protocol_metadata_get_negotiated_protocol(sec_protocol_metadata_t) -> UnsafePointer&lt;CChar>?

func sec_protocol_metadata_get_negotiated_protocol_version(sec_protocol_metadata_t) -> SSLProtocolDeprecated

func sec_protocol_metadata_get_negotiated_tls_ciphersuite(sec_protocol_metadata_t) -> tls_ciphersuite_t

func sec_protocol_metadata_get_negotiated_tls_protocol_version(sec_protocol_metadata_t) -> tls_protocol_version_t

func sec_protocol_metadata_get_server_name(sec_protocol_metadata_t) -> UnsafePointer&lt;CChar>?

func sec_protocol_metadata_peers_are_equal(sec_protocol_metadata_t, sec_protocol_metadata_t) -> Bool

func sec_protocol_options_add_pre_shared_key(sec_protocol_options_t, dispatch_data_t, dispatch_data_t)

func sec_protocol_options_add_tls_application_protocol(sec_protocol_options_t, UnsafePointer&lt;CChar>)

func sec_protocol_options_add_tls_ciphersuite(sec_protocol_options_t, SSLCipherSuite)Deprecated

func sec_protocol_options_add_tls_ciphersuite_group(sec_protocol_options_t, SSLCiphersuiteGroup)Deprecated

func sec_protocol_options_append_tls_ciphersuite(sec_protocol_options_t, tls_ciphersuite_t)

func sec_protocol_options_append_tls_ciphersuite_group(sec_protocol_options_t, tls_ciphersuite_group_t)

func sec_protocol_options_are_equal(sec_protocol_options_t, sec_protocol_options_t) -> Bool

func sec_protocol_options_get_default_max_dtls_protocol_version() -> tls_protocol_version_t

func sec_protocol_options_get_default_max_tls_protocol_version() -> tls_protocol_version_t

func sec_protocol_options_get_default_min_dtls_protocol_version() -> tls_protocol_version_t

func sec_protocol_options_get_default_min_tls_protocol_version() -> tls_protocol_version_t

func sec_protocol_options_set_challenge_block(sec_protocol_options_t, sec_protocol_challenge_t, dispatch_queue_t)

func sec_protocol_options_set_key_update_block(sec_protocol_options_t, sec_protocol_key_update_t, dispatch_queue_t)

func sec_protocol_options_set_local_identity(sec_protocol_options_t, sec_identity_t)

func sec_protocol_options_set_max_tls_protocol_version(sec_protocol_options_t, tls_protocol_version_t)

func sec_protocol_options_set_min_tls_protocol_version(sec_protocol_options_t, tls_protocol_version_t)

func sec_protocol_options_set_peer_authentication_required(sec_protocol_options_t, Bool)

func sec_protocol_options_set_pre_shared_key_selection_block(sec_protocol_options_t, sec_protocol_pre_shared_key_selection_t, dispatch_queue_t)

func sec_protocol_options_set_tls_diffie_hellman_parameters(sec_protocol_options_t, dispatch_data_t)Deprecated

func sec_protocol_options_set_tls_false_start_enabled(sec_protocol_options_t, Bool)

func sec_protocol_options_set_tls_is_fallback_attempt(sec_protocol_options_t, Bool)

func sec_protocol_options_set_tls_max_version(sec_protocol_options_t, SSLProtocol)Deprecated

func sec_protocol_options_set_tls_min_version(sec_protocol_options_t, SSLProtocol)Deprecated

func sec_protocol_options_set_tls_ocsp_enabled(sec_protocol_options_t, Bool)

func sec_protocol_options_set_tls_pre_shared_key_identity_hint(sec_protocol_options_t, dispatch_data_t)

func sec_protocol_options_set_tls_renegotiation_enabled(sec_protocol_options_t, Bool)

func sec_protocol_options_set_tls_resumption_enabled(sec_protocol_options_t, Bool)

func sec_protocol_options_set_tls_sct_enabled(sec_protocol_options_t, Bool)

func sec_protocol_options_set_tls_server_name(sec_protocol_options_t, UnsafePointer&lt;CChar>)

func sec_protocol_options_set_tls_tickets_enabled(sec_protocol_options_t, Bool)

func sec_protocol_options_set_verify_block(sec_protocol_options_t, sec_protocol_verify_t, dispatch_queue_t)

func sec_release(UnsafeMutableRawPointer!)

func sec_retain(UnsafeMutableRawPointer!) -> UnsafeMutableRawPointer!

func sec_trust_copy_ref(sec_trust_t) -> Unmanaged&lt;SecTrust>

func sec_trust_create(SecTrust) -> sec_trust_t?

### Macros

var errSecErrnoBase: Int32

var errSecErrnoLimit: Int32

var kKeychainSuffix: String

var kSystemKeychainDir: String

var kSystemKeychainName: String

var kSystemUnlockFile: String

### Type aliases

typealias SecAsn1Template

A structure that defines one element of a BER or DER encoding.

Deprecated

typealias sec_certificate_t

typealias sec_identity_t

typealias sec_object_t

A `sec_object` is a generic, ARC-able type wrapper for common CoreFoundation Security types.

typealias sec_protocol_challenge_complete_t

typealias sec_protocol_challenge_t

typealias sec_protocol_key_update_complete_t

typealias sec_protocol_key_update_t

typealias sec_protocol_metadata_t

A `sec_protocol_metadata` instance conatins read-only properties of a connected and configured security protocol. Clients use this object to read information about a protocol instance. Properties include, for example, the negotiated TLS version, ciphersuite, and peer certificates.

typealias sec_protocol_options_t

A `sec_protocol_options` instance is a container of options for security protocol instances, such as TLS. Protocol options are used to configure security protocols in the network stack. For example, clients may set the maximum and minimum allowed TLS versions through protocol options.

typealias sec_protocol_pre_shared_key_selection_complete_t

typealias sec_protocol_pre_shared_key_selection_t

typealias sec_protocol_verify_complete_t

typealias sec_protocol_verify_t

typealias sec_trust_t

These are os_object compatible and ARC-able wrappers around existing CoreFoundation Security types, including: SecTrustRef, SecIdentityRef, and SecCertificateRef. They allow clients to use these types in os_object-type APIs and data structures. The underlying CoreFoundation types may be extracted and used by clients as needed.

typealias sint16

typealias sint32

typealias sint64

typealias sint8

typealias uint16

typealias uint32

typealias uint64

typealias uint8

### Enumerations

struct extension_data_format

