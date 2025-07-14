

- Core Foundation
-  CFHash(\_:) 

Function

# CFHash(\_:)

Returns a code that can be used to identify an object in a hashing structure.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFHash(_ cf: CFTypeRef!) -> CFHashCode
```

## Parameters 

`cf`  

A CFType object to examine.

## Return Value

An integer of type CFHashCode that represents a hashing value for `cf`.

## Discussion

Two objects that are equal (as determined by the CFEqual(_:_:) function) have the same hashing value. However, the converse is not true: two objects with the same hashing value might not be equal. That is, hashing values are not necessarily unique.

The hashing value for an object might change from release to release or from platform to platform.

