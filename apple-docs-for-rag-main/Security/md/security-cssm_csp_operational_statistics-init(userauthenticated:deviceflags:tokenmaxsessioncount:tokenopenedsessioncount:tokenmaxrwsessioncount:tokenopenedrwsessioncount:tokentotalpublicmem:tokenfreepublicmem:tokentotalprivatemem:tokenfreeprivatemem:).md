

- Security
- cssm_csp_operational_statistics
-  init(UserAuthenticated:DeviceFlags:TokenMaxSessionCount:TokenOpenedSessionCount:TokenMaxRWSessionCount:TokenOpenedRWSessionCount:TokenTotalPublicMem:TokenFreePublicMem:TokenTotalPrivateMem:TokenFreePrivateMem:) 

Initializer

# init(UserAuthenticated:DeviceFlags:TokenMaxSessionCount:TokenOpenedSessionCount:TokenMaxRWSessionCount:TokenOpenedRWSessionCount:TokenTotalPublicMem:TokenFreePublicMem:TokenTotalPrivateMem:TokenFreePrivateMem:)

Mac Catalyst 13.0+macOS 10.0+

``` source
init(
    UserAuthenticated: CSSM_BOOL,
    DeviceFlags: CSSM_CSP_FLAGS,
    TokenMaxSessionCount: uint32,
    TokenOpenedSessionCount: uint32,
    TokenMaxRWSessionCount: uint32,
    TokenOpenedRWSessionCount: uint32,
    TokenTotalPublicMem: uint32,
    TokenFreePublicMem: uint32,
    TokenTotalPrivateMem: uint32,
    TokenFreePrivateMem: uint32
)
```

