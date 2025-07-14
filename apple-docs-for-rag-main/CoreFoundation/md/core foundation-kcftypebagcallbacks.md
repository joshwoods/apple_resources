

- Core Foundation
-  kCFTypeBagCallBacks 

Global Variable

# kCFTypeBagCallBacks

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
let kCFTypeBagCallBacks: CFBagCallBacks
```

## Discussion

Predefined CFBagCallBacks structure containing a set of callbacks appropriate for use when the values in a CFBag are all CFType-derived objects. The retain callback is `CFRetain`, the release callback is `CFRelease`, the copy callback is `CFCopyDescription`, the equal callback is `CFEqual`, and the hash callback is `CFHash`. Therefore, if you use this constant when creating the collection, items are automatically retained when added to the collection, and released when removed from the collection.

## See Also

### Constants

let kCFCopyStringBagCallBacks: CFBagCallBacks

Predefined CFBagCallBacks structure containing a set of callbacks appropriate for use when the values in a CFBag are all CFString objects. The bag makes immutable copies of the strings placed into it.

