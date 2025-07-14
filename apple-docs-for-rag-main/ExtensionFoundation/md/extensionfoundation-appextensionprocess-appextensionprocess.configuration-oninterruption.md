

- ExtensionFoundation
- AppExtensionProcess
- AppExtensionProcess.Configuration
-  onInterruption 

Instance Property

# onInterruption

A closure the system calles when an extension process exits.

macOS 13.0+

``` source
var onInterruption: () -> Void
```

## Discussion

A closure that the system calls if the extension process created from this configuration exits. The configuration sets this property to nil before it calls the handler block.

