

- Paravirtualized Graphics
- PGDeviceDescriptor
-  raiseInterrupt 

Instance Property

# raiseInterrupt

A handler that the system calls to raise an interrupt in the guest environment.

Mac Catalyst 14.0+macOS 11.0+

``` source
var raiseInterrupt: PGRaiseInterrupt? { get set }
```

## See Also

### Handling Interrupts

typealias PGRaiseInterrupt

The block signature for a routine that raises interrupts in the guest environment.

