

- GSS
-  Context Services 

API Collection

# Context Services

Use context services to manage secure operations between endpoints.

## Overview

You use these flags as input to gss_init_sec_context(_:_:_:_:_:_:_:_:_:_:_:_:_:) to request certain context services. You also receive them as output from both that function and gss_accept_sec_context(_:_:_:_:_:_:_:_:_:_:_:), indicating which services are actually engaged. Requesting a service does not guarantee its availability.

Because these flags represent the bits of an integer, you combine them with a bitwise `OR` and pull them apart using bitwise `AND`, as shown below.

```
OM_uint32 req_flags = GSS_C_DELEG_FLAG | GSS_C_MUTUAL_FLAG;
OM_uint32 ret_flags = 0;
//
// Call gss_init_sec_context() with req_flags; get ret_flags back
//
BOOL deleg  = (ret_flags & GSS_C_DELEG_FLAG)  ? YES : NO;
BOOL mutual = (ret_flags & GSS_C_MUTUAL_FLAG) ? YES : NO;
```

## Topics

### Flags

var GSS_C_DELEG_FLAG: Int32

A flag that permits delegation of the initiator’s credentials by the acceptor.

var GSS_C_MUTUAL_FLAG: Int32

A flag that authenticates the credentials of both initiator and acceptor.

var GSS_C_REPLAY_FLAG: Int32

A flag that detects repeated messages.

var GSS_C_SEQUENCE_FLAG: Int32

A flag that detects out of sequence messages.

var GSS_C_CONF_FLAG: Int32

A flag that makes confidentiality services (that is, encryption) available for transferred messages.

var GSS_C_INTEG_FLAG: Int32

A flag that makes integrity services (that is, cryptographic signatures) available for transferred messages.

var GSS_C_ANON_FLAG: Int32

A flag that ensures the initiator remains anonymous to the acceptor.

var GSS_C_PROT_READY_FLAG: Int32

A flag that provides an early indication of the availability of confidentiality and integrity services.

var GSS_C_TRANS_FLAG: Int32

A flag that indicates that a context can is exportable, for example to transfer it to another process on the same machine.

var GSS_C_DCE_STYLE: Int32

A flag that causes an extra AP reply to be sent from the client back to the server after receiving the server’s AP reply.

var GSS_C_IDENTIFY_FLAG: Int32

A flag that indicates identification of the client by name and ID only.

var GSS_C_EXTENDED_ERROR_FLAG: Int32

A flag that indicates that the client wants to be informed of extended error information.

var GSS_C_DELEG_POLICY_FLAG: Int32

A flag that indicates delegation is permissible if the mechanism policy allows it.

### Address Families

The constant definitions for channel-binding address families.

var GSS_C_AF_NS: Int32

The Xerox NS address type.

var GSS_C_AF_BSC: Int32

The BISYNC 2780/3780 address type.

var GSS_C_AF_DLI: Int32

The direct data link interface address type.

var GSS_C_AF_DSS: Int32

The distributed system services address type.

var GSS_C_AF_LAT: Int32

The LAT address type.

var GSS_C_AF_NBS: Int32

The nbs address type.

var GSS_C_AF_OSI: Int32

The OSI TP4 address type.

var GSS_C_AF_PUP: Int32

The PUP protocols (for example, BSP) address type.

var GSS_C_AF_SNA: Int32

The IBM SNA address type.

var GSS_C_AF_X25: Int32

The X.25 address type.

var GSS_C_AF_ECMA: Int32

The ECMA address type.

var GSS_C_AF_INET: Int32

The Internet (for example, IP) address type.

var GSS_C_AF_CCITT: Int32

The CCITT protocols address type.

var GSS_C_AF_CHAOS: Int32

The MIT CHAOS protocol address type.

var GSS_C_AF_INET6: Int32

The IPv6 address type.

var GSS_C_AF_LOCAL: Int32

The host-local address type.

var GSS_C_AF_DECnet: Int32

The DECnet address type.

var GSS_C_AF_HYLINK: Int32

The NSC Hyperchannel address type.

var GSS_C_AF_UNSPEC: Int32

The unspecified address type.

var GSS_C_AF_DATAKIT: Int32

The datakit protocols address type.

var GSS_C_AF_IMPLINK: Int32

ARPAnet IMP address type.

var GSS_C_AF_NULLADDR: Int32

No address specified.

var GSS_C_AF_APPLETALK: Int32

The AppleTalk address type.

### Apple Source App Keys

The keys used in the dictionary specified by the kGSSICAppleSourceApp key.

var kGSSICAppleSourceAppPID: String

A number that indicates the process ID of the app.

var kGSSICAppleSourceAppAuditToken: String

The audit token of the app’s process.

var kGSSICAppleSourceAppSigningIdentity: String

The bundle signing identity of the app.

### Channel Bindings

typealias gss_ctx_id_t

A pointer to an opaque type that you use to communicate context pointers with GSS-API functions.

struct gss_channel_bindings_struct

The structure defining a channel bindings descriptor that specifies the communications channel used to carry a context.

typealias gss_channel_bindings_t

A pointer to a channel bindings descriptor that specifies the communications channel used to carry a context.

typealias gss_const_channel_bindings_t

A pointer to an immutable channel bindings descriptor that you use to specify the communications channel used to carry a context.

### Creation and Deletion

func gss_init_sec_context(UnsafeMutablePointer&lt;OM_uint32>, gss_cred_id_t?, UnsafeMutablePointer&lt;gss_ctx_id_t?>, gss_name_t, gss_OID?, OM_uint32, OM_uint32, gss_channel_bindings_t?, gss_buffer_t?, UnsafeMutablePointer&lt;gss_OID?>?, gss_buffer_t, UnsafeMutablePointer&lt;OM_uint32>?, UnsafeMutablePointer&lt;OM_uint32>?) -> OM_uint32

Initiates a security context with a peer.

func gss_accept_sec_context(UnsafeMutablePointer&lt;OM_uint32>, UnsafeMutablePointer&lt;gss_ctx_id_t?>, gss_cred_id_t?, gss_buffer_t?, gss_channel_bindings_t?, UnsafeMutablePointer&lt;gss_name_t?>?, UnsafeMutablePointer&lt;gss_OID?>?, gss_buffer_t, UnsafeMutablePointer&lt;OM_uint32>?, UnsafeMutablePointer&lt;OM_uint32>?, UnsafeMutablePointer&lt;gss_cred_id_t?>?) -> OM_uint32

Accepts a security context initiated by a peer.

func gss_delete_sec_context(UnsafeMutablePointer&lt;OM_uint32>, UnsafeMutablePointer&lt;gss_ctx_id_t?>, gss_buffer_t?) -> OM_uint32

Deletes a security context.

func gss_release_cred(UnsafeMutablePointer&lt;OM_uint32>, UnsafeMutablePointer&lt;gss_cred_id_t?>) -> OM_uint32

Releases the memory of a credential.

func gss_process_context_token(UnsafeMutablePointer&lt;OM_uint32>, gss_ctx_id_t, gss_buffer_t) -> OM_uint32

Processes a token from a peer asynchronously.

func gss_set_sec_context_option(UnsafeMutablePointer&lt;OM_uint32>, UnsafeMutablePointer&lt;gss_ctx_id_t>?, gss_OID, gss_buffer_t?) -> OM_uint32

Sets an option on a context.

### Inquiry and Limits

func gss_context_time(UnsafeMutablePointer&lt;OM_uint32>, gss_ctx_id_t, UnsafeMutablePointer&lt;OM_uint32>) -> OM_uint32

Returns the amount of time remaining before a context expires.

func gss_inquire_context(UnsafeMutablePointer&lt;OM_uint32>, gss_ctx_id_t, UnsafeMutablePointer&lt;gss_name_t?>?, UnsafeMutablePointer&lt;gss_name_t?>?, UnsafeMutablePointer&lt;OM_uint32>?, UnsafeMutablePointer&lt;gss_OID?>?, UnsafeMutablePointer&lt;OM_uint32>?, UnsafeMutablePointer&lt;Int32>?, UnsafeMutablePointer&lt;Int32>?) -> OM_uint32

Returns information about a security context.

func gss_inquire_sec_context_by_oid(UnsafeMutablePointer&lt;OM_uint32>, gss_ctx_id_t, gss_OID, UnsafeMutablePointer&lt;gss_buffer_set_t>?) -> OM_uint32

Returns information about a particular part of a context.

func gss_wrap_size_limit(UnsafeMutablePointer&lt;OM_uint32>, gss_ctx_id_t, Int32, gss_qop_t, OM_uint32, UnsafeMutablePointer&lt;OM_uint32>) -> OM_uint32

Returns the largest allowable wrap size for a given set of constraints.

### Import and Export

func gss_export_sec_context(UnsafeMutablePointer&lt;OM_uint32>, UnsafeMutablePointer&lt;gss_ctx_id_t?>, gss_buffer_t?) -> OM_uint32

Transfers a security context to another process.

func gss_import_sec_context(UnsafeMutablePointer&lt;OM_uint32>, gss_buffer_t, UnsafeMutablePointer&lt;gss_ctx_id_t?>) -> OM_uint32

Imports a security context from another process.

## See Also

### Memory and Context

Allocating and Releasing Objects

Manage memory and object lifetimes.

Function Status

Evaluate return values that most GSS-API functions use to indicate the outcome of an operation.

Buffer Management

Allocate and deallocate buffers with structures that hold a variety of data.

