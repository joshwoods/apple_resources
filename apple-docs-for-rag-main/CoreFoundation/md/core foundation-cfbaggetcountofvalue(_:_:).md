

- Core Foundation
-  CFBagGetCountOfValue(\_:\_:) 

Function

# CFBagGetCountOfValue(\_:\_:)

Returns the number of times a value occurs in a bag.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBagGetCountOfValue(
    _ theBag: CFBag!,
    _ value: UnsafeRawPointer!
) -> CFIndex
```

## Parameters 

`theBag`  

The bag to examine.

`value`  

The value for which to find matches in `theBag`. The equal callback provided when `theBag` was created is used to compare. If the equal callback was `NULL`, pointer equality (in C, ==) is used. If `value`, or any other value in `theBag`, is not understood by the equal callback, the behavior is undefined.

## Return Value

The number of times `value` occurs in `theBag`.

## See Also

### Examining a Bag

func CFBagContainsValue(CFBag!, UnsafeRawPointer!) -> Bool

Reports whether or not a value is in a bag.

func CFBagGetCount(CFBag!) -> CFIndex

Returns the number of values currently in a bag.

func CFBagGetValue(CFBag!, UnsafeRawPointer!) -> UnsafeRawPointer!

Returns a requested value from a bag.

func CFBagGetValueIfPresent(CFBag!, UnsafeRawPointer!, UnsafeMutablePointer&lt;UnsafeRawPointer?>!) -> Bool

Reports whether or not a value is in a bag, and returns that value indirectly if it exists.

func CFBagGetValues(CFBag!, UnsafeMutablePointer&lt;UnsafeRawPointer?>!)

Fills a buffer with values from a bag.

