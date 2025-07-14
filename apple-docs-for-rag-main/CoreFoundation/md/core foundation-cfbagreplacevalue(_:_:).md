

- Core Foundation
-  CFBagReplaceValue(\_:\_:) 

Function

# CFBagReplaceValue(\_:\_:)

Replaces a value in a mutable bag.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBagReplaceValue(
    _ theBag: CFMutableBag!,
    _ value: UnsafeRawPointer!
)
```

## Parameters 

`theBag`  

The bag from which `value` is to be replaced.

`value`  

The value to be replaced in the collection. If this value does not already exist in the collection, the function does nothing. You may pass the value itself instead of a pointer if it is pointer-size or less. The equal callback provided when `theBag` was created is used to compare. If the equal callback was `NULL`, pointer equality (in C, ==) is used. If `value`, or any other value in `theBag`, is not understood by the equal callback, the behavior is undefined.

## Discussion

Depending on the implementation of the equal callback specified when creating `theBag`, the object that is replaced by `value` may not have the same pointer equality.

## See Also

### Modifying a Mutable Bag

func CFBagAddValue(CFMutableBag!, UnsafeRawPointer!)

Adds a value to a mutable bag.

func CFBagRemoveAllValues(CFMutableBag!)

Removes all values from a mutable bag.

func CFBagRemoveValue(CFMutableBag!, UnsafeRawPointer!)

Removes a value from a mutable bag.

func CFBagSetValue(CFMutableBag!, UnsafeRawPointer!)

Sets a value in a mutable bag.

