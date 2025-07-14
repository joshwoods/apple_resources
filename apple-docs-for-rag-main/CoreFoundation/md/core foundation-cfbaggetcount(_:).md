

- Core Foundation
-  CFBagGetCount(\_:) 

Function

# CFBagGetCount(\_:)

Returns the number of values currently in a bag.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFBagGetCount(_ theBag: CFBag!) -> CFIndex
```

## Parameters 

`theBag`  

The bag to examine.

## Return Value

The number of values in `theBag`.

## See Also

### Examining a Bag

func CFBagContainsValue(CFBag!, UnsafeRawPointer!) -> Bool

Reports whether or not a value is in a bag.

func CFBagGetCountOfValue(CFBag!, UnsafeRawPointer!) -> CFIndex

Returns the number of times a value occurs in a bag.

func CFBagGetValue(CFBag!, UnsafeRawPointer!) -> UnsafeRawPointer!

Returns a requested value from a bag.

func CFBagGetValueIfPresent(CFBag!, UnsafeRawPointer!, UnsafeMutablePointer&lt;UnsafeRawPointer?>!) -> Bool

Reports whether or not a value is in a bag, and returns that value indirectly if it exists.

func CFBagGetValues(CFBag!, UnsafeMutablePointer&lt;UnsafeRawPointer?>!)

Fills a buffer with values from a bag.

