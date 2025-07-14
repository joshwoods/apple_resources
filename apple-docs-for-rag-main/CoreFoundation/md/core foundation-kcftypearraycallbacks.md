

- Core Foundation
-  kCFTypeArrayCallBacks 

Global Variable

# kCFTypeArrayCallBacks

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
let kCFTypeArrayCallBacks: CFArrayCallBacks
```

## Discussion

Predefined CFArrayCallBacks structure containing a set of callbacks appropriate for use when the values in a CFArray are all CFType-derived objects. The retain callback is `CFRetain`, the release callback is `CFRelease`, the copy callback is `CFCopyDescription`, and the equal callback is `CFEqual`. Therefore, if you use this constant when creating the collection, items are automatically retained when added to the collection, and released when removed from the collection.

