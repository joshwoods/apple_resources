

- Core Foundation
-  CFByteOrder 

Type Alias

# CFByteOrder

Flags that identify byte order.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CFByteOrder = CFIndex
```

## Topics

### Constants

var CFByteOrderUnknown: __CFByteOrder

The byte order is unknown.

var CFByteOrderLittleEndian: __CFByteOrder

Multi-byte values are stored with the least-significant bytes stored first. Pentium CPUs are little endian.

var CFByteOrderBigEndian: __CFByteOrder

Multi-byte values are stored with the most-significant bytes stored first. PowerPC CPUs are big endian.

