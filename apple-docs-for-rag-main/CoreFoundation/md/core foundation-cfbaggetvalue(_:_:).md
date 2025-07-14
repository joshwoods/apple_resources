

- Core Foundation
-  CFBagGetValue(\_:\_:) 

Function

# CFBagGetValue(\_:\_:)

Returns a requested value from a bag.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBagGetValue(
    _ theBag: CFBag!,
    _ value: UnsafeRawPointer!
) -> UnsafeRawPointer!
```

## Parameters 

`theBag`  

The bag to examine.

`value`  

The value for which to find matches in `theBag`. The equal callback provided when `theBag` was created is used to compare. If the equal callback was `NULL`, pointer equality (in C, ==) is used. If `value`, or any other value in `theBag`, is not understood by the equal callback, the behavior is undefined.

## Return Value

A pointer to `value`, or `NULL` if `value` is not in `theBag`. If the value is a Core Foundation object, ownership follows the The Get Rule.

## Discussion

Depending on the implementation of the equal callback specified when creating `theBag`, the value returned may not have the same pointer equality as `value`.

## See Also

### Examining a Bag

func CFBagContainsValue(CFBag!, UnsafeRawPointer!) -> Bool

Reports whether or not a value is in a bag.

func CFBagGetCount(CFBag!) -> CFIndex

Returns the number of values currently in a bag.

func CFBagGetCountOfValue(CFBag!, UnsafeRawPointer!) -> CFIndex

Returns the number of times a value occurs in a bag.

func CFBagGetValueIfPresent(CFBag!, UnsafeRawPointer!, UnsafeMutablePointer&lt;UnsafeRawPointer?>!) -> Bool

Reports whether or not a value is in a bag, and returns that value indirectly if it exists.

func CFBagGetValues(CFBag!, UnsafeMutablePointer&lt;UnsafeRawPointer?>!)

Fills a buffer with values from a bag.

