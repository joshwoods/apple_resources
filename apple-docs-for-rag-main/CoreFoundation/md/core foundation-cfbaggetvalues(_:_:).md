

- Core Foundation
-  CFBagGetValues(\_:\_:) 

Function

# CFBagGetValues(\_:\_:)

Fills a buffer with values from a bag.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBagGetValues(
    _ theBag: CFBag!,
    _ values: UnsafeMutablePointer!
)
```

## Parameters 

`theBag`  

The bag to examine.

`values`  

A C array of pointer-sized values to be filled with values from `theBag`. The value must be a valid C array of the appropriate type and size (that is, a size equal to the count of `theBag`).

## See Also

### Examining a Bag

func CFBagContainsValue(CFBag!, UnsafeRawPointer!) -> Bool

Reports whether or not a value is in a bag.

func CFBagGetCount(CFBag!) -> CFIndex

Returns the number of values currently in a bag.

func CFBagGetCountOfValue(CFBag!, UnsafeRawPointer!) -> CFIndex

Returns the number of times a value occurs in a bag.

func CFBagGetValue(CFBag!, UnsafeRawPointer!) -> UnsafeRawPointer!

Returns a requested value from a bag.

func CFBagGetValueIfPresent(CFBag!, UnsafeRawPointer!, UnsafeMutablePointer&lt;UnsafeRawPointer?>!) -> Bool

Reports whether or not a value is in a bag, and returns that value indirectly if it exists.

