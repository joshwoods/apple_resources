

- Security
-  CSSM_APPLE_TP_SSL_OPTIONS 

Structure

# CSSM_APPLE_TP_SSL_OPTIONS

macOS 10.0+

``` source
struct CSSM_APPLE_TP_SSL_OPTIONS
```

## Topics

### Initializers

init()

init(Version: uint32, ServerNameLen: uint32, ServerName: UnsafePointer&lt;CChar>!, Flags: uint32)

### Instance Properties

var Flags: uint32

var ServerName: UnsafePointer&lt;CChar>!

var ServerNameLen: uint32

var Version: uint32

## Relationships

### Conforms To

- BitwiseCopyable

