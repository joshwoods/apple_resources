

- Core Foundation
-  kCFTypeSetCallBacks 

Global Variable

# kCFTypeSetCallBacks

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
let kCFTypeSetCallBacks: CFSetCallBacks
```

## Discussion

Predefined CFSetCallBacks structure containing a set of callbacks appropriate for use when the values in a CFSet are all CFType-derived objects. The retain callback is CFRetain, the release callback is CFRelease, the copy callback is CFCopyDescription(_:), the equal callback is CFEqual(_:_:), and the hash callback is CFHash(_:). Therefore, if you use this constant when creating the collection, items are automatically retained when added to the collection, and released when removed from the collection.

## See Also

### Constants

let kCFCopyStringSetCallBacks: CFSetCallBacks

Predefined CFSetCallBacks structure containing a set of callbacks appropriate for use when the values in a set are all CFString objects. The retain callback makes an immutable copy of strings added to the set.

