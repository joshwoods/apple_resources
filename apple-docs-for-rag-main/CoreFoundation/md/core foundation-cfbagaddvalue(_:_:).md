

- Core Foundation
-  CFBagAddValue(\_:\_:) 

Function

# CFBagAddValue(\_:\_:)

Adds a value to a mutable bag.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBagAddValue(
    _ theBag: CFMutableBag!,
    _ value: UnsafeRawPointer!
)
```

## Parameters 

`theBag`  

The bag to which `value` is added.

`value`  

A CFType object or a pointer value to add to `theBag` (or the value itself, if it fits into the size of a pointer).

## Discussion

The `value` parameter is retained by `theBag` using the retain callback provided when `theBag` was created. If `value` is not of the type expected by the retain callback, the behavior is undefined. If `value` already exists in the collection, it is simply retained again—no memory is allocated for the added value. Use a CFSet object if you don’t want duplicate values in your collection.

## See Also

### Modifying a Mutable Bag

func CFBagRemoveAllValues(CFMutableBag!)

Removes all values from a mutable bag.

func CFBagRemoveValue(CFMutableBag!, UnsafeRawPointer!)

Removes a value from a mutable bag.

func CFBagReplaceValue(CFMutableBag!, UnsafeRawPointer!)

Replaces a value in a mutable bag.

func CFBagSetValue(CFMutableBag!, UnsafeRawPointer!)

Sets a value in a mutable bag.

