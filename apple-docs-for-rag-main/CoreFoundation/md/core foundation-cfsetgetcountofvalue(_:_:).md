

- Core Foundation
-  CFSetGetCountOfValue(\_:\_:) 

Function

# CFSetGetCountOfValue(\_:\_:)

Returns the number of values in a set that match a given value.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFSetGetCountOfValue(
    _ theSet: CFSet!,
    _ value: UnsafeRawPointer!
) -> CFIndex
```

## Parameters 

`theSet`  

The set to examine.

`value`  

The value for which to search in `theSet`. Comparisons are made using the equal callback provided when `theSet` was created. If the equal callback was `NULL`, pointer equality (in C, ==) is used.

## Return Value

The number of times `value` occurs in `theSet`. By definition, sets can not contain duplicate values, so returns `1` if `value` is contained in `theSet`, otherwise `0`.

## Discussion

This function uses the equal callback. `value` and all elements in the set must be understood by the equal callback.

## See Also

### Examining a Set

func CFSetContainsValue(CFSet!, UnsafeRawPointer!) -> Bool

Returns a Boolean that indicates whether a set contains a given value.

func CFSetGetCount(CFSet!) -> CFIndex

Returns the number of values currently in a set.

func CFSetGetValue(CFSet!, UnsafeRawPointer!) -> UnsafeRawPointer!

Obtains a specified value from a set.

func CFSetGetValueIfPresent(CFSet!, UnsafeRawPointer!, UnsafeMutablePointer&lt;UnsafeRawPointer?>!) -> Bool

Reports whether or not a value is in a set, and if it exists returns the value indirectly.

func CFSetGetValues(CFSet!, UnsafeMutablePointer&lt;UnsafeRawPointer?>!)

Obtains all values in a set.

