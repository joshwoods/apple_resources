

- GSS
-  GSS_C_ACCEPT 

Global Variable

# GSS_C_ACCEPT

The value that indicates a credential that can accept a security context.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.0+macOS 10.14+visionOS 1.0+

``` source
var GSS_C_ACCEPT: Int32 { get }
```

## See Also

### Credential Masks and Macros

var GSS_C_INDEFINITE: UInt

The value that indicates the maximum permitted lifetime when used in a time request.

var GSS_C_INITIATE: Int32

The value that indicates a credential that can initiate a security context.

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

