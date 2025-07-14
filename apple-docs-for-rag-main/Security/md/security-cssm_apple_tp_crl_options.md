

- Security
-  CSSM_APPLE_TP_CRL_OPTIONS 

Structure

# CSSM_APPLE_TP_CRL_OPTIONS

macOS 10.0+

``` source
struct CSSM_APPLE_TP_CRL_OPTIONS
```

## Topics

### Initializers

init()

init(Version: uint32, CrlFlags: CSSM_APPLE_TP_CRL_OPT_FLAGS, crlStore: UnsafeMutablePointer&lt;cssm_dl_db_handle>!)

### Instance Properties

var CrlFlags: CSSM_APPLE_TP_CRL_OPT_FLAGS

var Version: uint32

var crlStore: UnsafeMutablePointer&lt;cssm_dl_db_handle>!

## Relationships

### Conforms To

- BitwiseCopyable

