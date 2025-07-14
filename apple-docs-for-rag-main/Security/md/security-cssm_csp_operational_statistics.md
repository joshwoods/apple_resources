

- Security
-  cssm_csp_operational_statistics 

Structure

# cssm_csp_operational_statistics

Mac Catalyst 13.0+macOS 10.0+

``` source
struct cssm_csp_operational_statistics
```

## Topics

### Initializers

init()

init(UserAuthenticated: CSSM_BOOL, DeviceFlags: CSSM_CSP_FLAGS, TokenMaxSessionCount: uint32, TokenOpenedSessionCount: uint32, TokenMaxRWSessionCount: uint32, TokenOpenedRWSessionCount: uint32, TokenTotalPublicMem: uint32, TokenFreePublicMem: uint32, TokenTotalPrivateMem: uint32, TokenFreePrivateMem: uint32)

### Instance Properties

var DeviceFlags: CSSM_CSP_FLAGS

var TokenFreePrivateMem: uint32

var TokenFreePublicMem: uint32

var TokenMaxRWSessionCount: uint32

var TokenMaxSessionCount: uint32

var TokenOpenedRWSessionCount: uint32

var TokenOpenedSessionCount: uint32

var TokenTotalPrivateMem: uint32

var TokenTotalPublicMem: uint32

var UserAuthenticated: CSSM_BOOL

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

