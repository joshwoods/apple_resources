

- Paravirtualized Graphics
-  PGRaiseInterrupt 

Type Alias

# PGRaiseInterrupt

The block signature for a routine that raises interrupts in the guest environment.

Mac Catalyst 14.0+macOS 11.0+

``` source
typealias PGRaiseInterrupt = (UInt32) -> Void
```

## Parameters 

`vector `  

The MSI vector to raise the interrupt on.

## See Also

### Handling Interrupts

var raiseInterrupt: PGRaiseInterrupt?

A handler that the system calls to raise an interrupt in the guest environment.

