

- Security
-  CSSM_APPLE_TP_SMIME_OPTIONS 

Structure

# CSSM_APPLE_TP_SMIME_OPTIONS

macOS 10.0+

``` source
struct CSSM_APPLE_TP_SMIME_OPTIONS
```

## Topics

### Initializers

init()

init(Version: uint32, IntendedUsage: uint16, SenderEmailLen: uint32, SenderEmail: UnsafePointer&lt;CChar>!)

### Instance Properties

var IntendedUsage: uint16

var SenderEmail: UnsafePointer&lt;CChar>!

var SenderEmailLen: uint32

var Version: uint32

## Relationships

### Conforms To

- BitwiseCopyable

