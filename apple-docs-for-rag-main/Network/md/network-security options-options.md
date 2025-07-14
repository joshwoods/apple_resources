

- Network
-  Security Options 

# Security Options

Configure security options for TLS handshakes.

## Topics

### Configuring TLS Handshake Options

typealias sec_protocol_options_t = any OS_sec_protocol_options

A \`sec_protocol_options\` instance is a container of options for security protocol instances, such as TLS. Protocol options are used to configure security protocols in the network stack. For example, clients may set the maximum and minimum allowed TLS versions through protocol options.

protocol OS_sec_protocol_options : NSObjectProtocol

A \`sec_protocol_options\` instance is a container of options for security protocol instances, such as TLS. Protocol options are used to configure security protocols in the network stack. For example, clients may set the maximum and minimum allowed TLS versions through protocol options.

func sec_protocol_options_set_tls_server_name(_ options: sec_protocol_options_t, _ server_name: UnsafePointer&lt;CChar>)

func sec_protocol_options_add_pre_shared_key(_ options: sec_protocol_options_t, _ psk: dispatch_data_t, _ psk_identity: dispatch_data_t)

func sec_protocol_options_add_tls_application_protocol(_ options: sec_protocol_options_t, _ application_protocol: UnsafePointer&lt;CChar>)

func sec_protocol_options_append_tls_ciphersuite(_ options: sec_protocol_options_t, _ ciphersuite: tls_ciphersuite_t)

func sec_protocol_options_append_tls_ciphersuite_group(_ options: sec_protocol_options_t, _ group: tls_ciphersuite_group_t)

func sec_protocol_options_add_tls_ciphersuite(_ options: sec_protocol_options_t, _ ciphersuite: SSLCipherSuite)

Deprecated

func sec_protocol_options_add_tls_ciphersuite_group(_ options: sec_protocol_options_t, _ group: SSLCiphersuiteGroup)

Deprecated

func sec_protocol_options_set_tls_diffie_hellman_parameters(_ options: sec_protocol_options_t, _ params: dispatch_data_t)

Deprecated

func sec_protocol_options_are_equal(_ optionsA: sec_protocol_options_t, _ optionsB: sec_protocol_options_t) -> Bool

### Configuring TLS Versions

func sec_protocol_options_set_min_tls_protocol_version(_ options: sec_protocol_options_t, _ version: tls_protocol_version_t)

func sec_protocol_options_set_max_tls_protocol_version(_ options: sec_protocol_options_t, _ version: tls_protocol_version_t)

func sec_protocol_options_get_default_min_tls_protocol_version() -> tls_protocol_version_t

func sec_protocol_options_get_default_max_tls_protocol_version() -> tls_protocol_version_t

func sec_protocol_options_get_default_min_dtls_protocol_version() -> tls_protocol_version_t

func sec_protocol_options_get_default_max_dtls_protocol_version() -> tls_protocol_version_t

func sec_protocol_options_set_tls_min_version(_ options: sec_protocol_options_t, _ version: SSLProtocol)

Deprecated

func sec_protocol_options_set_tls_max_version(_ options: sec_protocol_options_t, _ version: SSLProtocol)

Deprecated

### Configuring TLS Behavior

func sec_protocol_options_set_tls_resumption_enabled(_ options: sec_protocol_options_t, _ resumption_enabled: Bool)

func sec_protocol_options_set_tls_tickets_enabled(_ options: sec_protocol_options_t, _ tickets_enabled: Bool)

func sec_protocol_options_set_tls_false_start_enabled(_ options: sec_protocol_options_t, _ false_start_enabled: Bool)

func sec_protocol_options_set_tls_sct_enabled(_ options: sec_protocol_options_t, _ sct_enabled: Bool)

func sec_protocol_options_set_tls_ocsp_enabled(_ options: sec_protocol_options_t, _ ocsp_enabled: Bool)

func sec_protocol_options_set_tls_renegotiation_enabled(_ options: sec_protocol_options_t, _ renegotiation_enabled: Bool)

func sec_protocol_options_set_peer_authentication_required(_ options: sec_protocol_options_t, _ peer_authentication_required: Bool)

func sec_protocol_options_set_tls_is_fallback_attempt(_ options: sec_protocol_options_t, _ is_fallback_attempt: Bool)

func sec_protocol_options_set_tls_pre_shared_key_identity_hint(_ options: sec_protocol_options_t, _ psk_identity_hint: dispatch_data_t)

### Handling TLS Events

func sec_protocol_options_set_verify_block(_ options: sec_protocol_options_t, _ verify_block: @escaping sec_protocol_verify_t, _ verify_block_queue: dispatch_queue_t)

typealias sec_protocol_verify_t = (sec_protocol_metadata_t, sec_trust_t, @escaping sec_protocol_verify_complete_t) -> Void

typealias sec_protocol_verify_complete_t = (Bool) -> Void

func sec_protocol_options_set_challenge_block(_ options: sec_protocol_options_t, _ challenge_block: @escaping sec_protocol_challenge_t, _ challenge_queue: dispatch_queue_t)

typealias sec_protocol_challenge_t = (sec_protocol_metadata_t, @escaping sec_protocol_challenge_complete_t) -> Void

typealias sec_protocol_challenge_complete_t = (sec_identity_t?) -> Void

func sec_protocol_options_set_key_update_block(_ options: sec_protocol_options_t, _ key_update_block: @escaping sec_protocol_key_update_t, _ key_update_queue: dispatch_queue_t)

typealias sec_protocol_key_update_t = (sec_protocol_metadata_t, @escaping sec_protocol_key_update_complete_t) -> Void

typealias sec_protocol_key_update_complete_t = () -> Void

func sec_protocol_options_set_pre_shared_key_selection_block(_ options: sec_protocol_options_t, _ psk_selection_block: @escaping sec_protocol_pre_shared_key_selection_t, _ psk_selection_queue: dispatch_queue_t)

typealias sec_protocol_pre_shared_key_selection_t = (sec_protocol_metadata_t, dispatch_data_t?, @escaping sec_protocol_pre_shared_key_selection_complete_t) -> Void

typealias sec_protocol_pre_shared_key_selection_complete_t = (dispatch_data_t?) -> Void

### Inspecting TLS State

typealias sec_protocol_metadata_t = any OS_sec_protocol_metadata

A \`sec_protocol_metadata\` instance conatins read-only properties of a connected and configured security protocol. Clients use this object to read information about a protocol instance. Properties include, for example, the negotiated TLS version, ciphersuite, and peer certificates.

protocol OS_sec_protocol_metadata : NSObjectProtocol

A \`sec_protocol_metadata\` instance conatins read-only properties of a connected and configured security protocol. Clients use this object to read information about a protocol instance. Properties include, for example, the negotiated TLS version, ciphersuite, and peer certificates.

func sec_protocol_metadata_get_negotiated_protocol(_ metadata: sec_protocol_metadata_t) -> UnsafePointer&lt;CChar>?

func sec_protocol_metadata_get_server_name(_ metadata: sec_protocol_metadata_t) -> UnsafePointer&lt;CChar>?

func sec_protocol_metadata_get_negotiated_tls_protocol_version(_ metadata: sec_protocol_metadata_t) -> tls_protocol_version_t

func sec_protocol_metadata_get_negotiated_tls_ciphersuite(_ metadata: sec_protocol_metadata_t) -> tls_ciphersuite_t

func sec_protocol_metadata_get_negotiated_protocol_version(_ metadata: sec_protocol_metadata_t) -> SSLProtocol

Deprecated

func sec_protocol_metadata_get_negotiated_ciphersuite(_ metadata: sec_protocol_metadata_t) -> SSLCipherSuite

Deprecated

func sec_protocol_metadata_get_early_data_accepted(_ metadata: sec_protocol_metadata_t) -> Bool

func sec_protocol_metadata_copy_peer_public_key(_ metadata: sec_protocol_metadata_t) -> dispatch_data_t?

### Handling TLS Challenges

func sec_protocol_metadata_access_distinguished_names(_ metadata: sec_protocol_metadata_t, _ handler: @escaping (dispatch_data_t) -> Void) -> Bool

func sec_protocol_metadata_access_ocsp_response(_ metadata: sec_protocol_metadata_t, _ handler: @escaping (dispatch_data_t) -> Void) -> Bool

func sec_protocol_metadata_access_peer_certificate_chain(_ metadata: sec_protocol_metadata_t, _ handler: @escaping (sec_certificate_t) -> Void) -> Bool

func sec_protocol_metadata_access_supported_signature_algorithms(_ metadata: sec_protocol_metadata_t, _ handler: @escaping (UInt16) -> Void) -> Bool

func sec_protocol_metadata_access_pre_shared_keys(_ metadata: sec_protocol_metadata_t, _ handler: @escaping (dispatch_data_t, dispatch_data_t) -> Void) -> Bool

func sec_protocol_metadata_create_secret(_ metadata: sec_protocol_metadata_t, _ label_len: Int, _ label: UnsafePointer&lt;CChar>, _ exporter_length: Int) -> dispatch_data_t?

func sec_protocol_metadata_create_secret_with_context(_ metadata: sec_protocol_metadata_t, _ label_len: Int, _ label: UnsafePointer&lt;CChar>, _ context_len: Int, _ context: UnsafePointer&lt;UInt8>, _ exporter_length: Int) -> dispatch_data_t?

func sec_protocol_metadata_peers_are_equal(_ metadataA: sec_protocol_metadata_t, _ metadataB: sec_protocol_metadata_t) -> Bool

func sec_protocol_metadata_challenge_parameters_are_equal(_ metadataA: sec_protocol_metadata_t, _ metadataB: sec_protocol_metadata_t) -> Bool

### Handling Certificates

typealias sec_certificate_t = any OS_sec_certificate

protocol OS_sec_certificate : NSObjectProtocol

func sec_certificate_create(_ certificate: SecCertificate) -> sec_certificate_t?

func sec_certificate_copy_ref(_ certificate: sec_certificate_t) -> Unmanaged&lt;SecCertificate>

### Handling Identities

func sec_protocol_options_set_local_identity(_ options: sec_protocol_options_t, _ identity: sec_identity_t)

typealias sec_identity_t = any OS_sec_identity

protocol OS_sec_identity : NSObjectProtocol

func sec_identity_create(_ identity: SecIdentity) -> sec_identity_t?

func sec_identity_create_with_certificates(_ identity: SecIdentity, _ certificates: CFArray) -> sec_identity_t?

func sec_identity_copy_ref(_ identity: sec_identity_t) -> Unmanaged&lt;SecIdentity>?

func sec_identity_access_certificates(_ identity: sec_identity_t, _ handler: @escaping (sec_certificate_t) -> Void) -> Bool

func sec_identity_copy_certificates_ref(_ identity: sec_identity_t) -> Unmanaged&lt;CFArray>?

### Handling Trust

typealias sec_trust_t = any OS_sec_trust

These are os_object compatible and ARC-able wrappers around existing CoreFoundation Security types, including: SecTrustRef, SecIdentityRef, and SecCertificateRef. They allow clients to use these types in os_object-type APIs and data structures. The underlying CoreFoundation types may be extracted and used by clients as needed.

protocol OS_sec_trust : NSObjectProtocol

These are os_object compatible and ARC-able wrappers around existing CoreFoundation Security types, including: SecTrustRef, SecIdentityRef, and SecCertificateRef. They allow clients to use these types in os_object-type APIs and data structures. The underlying CoreFoundation types may be extracted and used by clients as needed.

func sec_trust_create(_ trust: SecTrust) -> sec_trust_t?

func sec_trust_copy_ref(_ trust: sec_trust_t) -> Unmanaged&lt;SecTrust>

### Managing Security Objects

func sec_release(_ obj: UnsafeMutableRawPointer!)

func sec_retain(_ obj: UnsafeMutableRawPointer!) -> UnsafeMutableRawPointer!

typealias sec_object_t = any OS_sec_object

A \`sec_object\` is a generic, ARC-able type wrapper for common CoreFoundation Security types.

protocol OS_sec_object : NSObjectProtocol

A \`sec_object\` is a generic, ARC-able type wrapper for common CoreFoundation Security types.

## See Also

### Network Security and Privacy

Privacy Management

Configure parameters related to user privacy.

Creating an Identity for Local Network TLS

Learn how to create and use a digital identity in your application for local network TLS.

