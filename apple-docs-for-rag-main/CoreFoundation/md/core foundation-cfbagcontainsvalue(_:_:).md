

- Core Foundation
-  CFBagContainsValue(\_:\_:) 

Function

# CFBagContainsValue(\_:\_:)

Reports whether or not a value is in a bag.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBagContainsValue(
    _ theBag: CFBag!,
    _ value: UnsafeRawPointer!
) -> Bool
```

## Parameters 

`theBag`  

The bag to examine.

`value`  

The value to match in `theBag`. The equal callback provided when `theBag` was created is used to compare. If the equal callback was `NULL`, pointer equality (in C, ==) is used. If `value`, or any other value in `theBag`, is not understood by the equal callback, the behavior is undefined.

## Return Value

`true` if `value` is contained in `theBag`, otherwise `false`.

## See Also

### Examining a Bag

func CFBagGetCount(CFBag!) -> CFIndex

Returns the number of values currently in a bag.

func CFBagGetCountOfValue(CFBag!, UnsafeRawPointer!) -> CFIndex

Returns the number of times a value occurs in a bag.

func CFBagGetValue(CFBag!, UnsafeRawPointer!) -> UnsafeRawPointer!

Returns a requested value from a bag.

func CFBagGetValueIfPresent(CFBag!, UnsafeRawPointer!, UnsafeMutablePointer&lt;UnsafeRawPointer?>!) -> Bool

Reports whether or not a value is in a bag, and returns that value indirectly if it exists.

func CFBagGetValues(CFBag!, UnsafeMutablePointer&lt;UnsafeRawPointer?>!)

Fills a buffer with values from a bag.

