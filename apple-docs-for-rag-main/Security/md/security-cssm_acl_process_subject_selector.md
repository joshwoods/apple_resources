

- Security
-  cssm_acl_process_subject_selector 

Structure

# cssm_acl_process_subject_selector

macOS 10.0+

``` source
struct cssm_acl_process_subject_selector
```

## Topics

### Initializers

init()

init(version: uint16, mask: uint16, uid: uint32, gid: uint32)

### Instance Properties

var gid: uint32

var mask: uint16

var uid: uint32

var version: uint16

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

