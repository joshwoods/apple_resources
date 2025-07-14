

- Core Media
-  kCMBlockBufferPermitEmptyReferenceFlag 

Global Variable

# kCMBlockBufferPermitEmptyReferenceFlag

Passed to CMBlockBuffer and CMBlockBuffer to allow references into a `CMBlockBuffer` that may not yet be populated.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var kCMBlockBufferPermitEmptyReferenceFlag: CMBlockBufferFlags { get }
```

## See Also

### Constants

var kCMBlockBufferAssureMemoryNowFlag: CMBlockBufferFlags

When passed to routines that accept block allocators, causes the memory block to be allocated immediately.

var kCMBlockBufferAlwaysCopyDataFlag: CMBlockBufferFlags

Used with CMBlockBuffer to cause it to always produce an allocated copy of the desired data.

var kCMBlockBufferDontOptimizeDepthFlag: CMBlockBufferFlags

Passed to block buffers to suppress reference depth optimization.

