

- Core Foundation
-  CFBagRemoveValue(\_:\_:) 

Function

# CFBagRemoveValue(\_:\_:)

Removes a value from a mutable bag.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBagRemoveValue(
    _ theBag: CFMutableBag!,
    _ value: UnsafeRawPointer!
)
```

## Parameters 

`theBag`  

The bag from which `value` is to be removed.

`value`  

The value to be removed from the collection.

## See Also

### Modifying a Mutable Bag

func CFBagAddValue(CFMutableBag!, UnsafeRawPointer!)

Adds a value to a mutable bag.

func CFBagRemoveAllValues(CFMutableBag!)

Removes all values from a mutable bag.

func CFBagReplaceValue(CFMutableBag!, UnsafeRawPointer!)

Replaces a value in a mutable bag.

func CFBagSetValue(CFMutableBag!, UnsafeRawPointer!)

Sets a value in a mutable bag.

