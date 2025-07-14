

- Core Foundation
- CFArrayCallBacks
-  equal 

Instance Property

# equal

The callback used to compare values in the array for equality for some operations. If `NULL`, the collection will use pointer equality to compare values in the collection. See CFArrayEqualCallBack for a description of this callback.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var equal: CFArrayEqualCallBack!
```

