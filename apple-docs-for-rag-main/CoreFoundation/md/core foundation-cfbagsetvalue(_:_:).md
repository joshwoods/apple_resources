

- Core Foundation
-  CFBagSetValue(\_:\_:) 

Function

# CFBagSetValue(\_:\_:)

Sets a value in a mutable bag.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBagSetValue(
    _ theBag: CFMutableBag!,
    _ value: UnsafeRawPointer!
)
```

## Parameters 

`theBag`  

The bag in which `value` is to be set.

`value`  

The value to be set in the collection. If this value already exists in `theBag`, it is replaced. You may pass the value itself instead of a pointer to it if the value is pointer-size or less. If `theBag` is fixed-size and the value is beyond its capacity, the behavior is undefined.

## Discussion

Depending on the implementation of the equal callback specified when creating `theBag`, the value that is replaced by `value` may not have the same pointer equality.

## See Also

### Modifying a Mutable Bag

func CFBagAddValue(CFMutableBag!, UnsafeRawPointer!)

Adds a value to a mutable bag.

func CFBagRemoveAllValues(CFMutableBag!)

Removes all values from a mutable bag.

func CFBagRemoveValue(CFMutableBag!, UnsafeRawPointer!)

Removes a value from a mutable bag.

func CFBagReplaceValue(CFMutableBag!, UnsafeRawPointer!)

Replaces a value in a mutable bag.

