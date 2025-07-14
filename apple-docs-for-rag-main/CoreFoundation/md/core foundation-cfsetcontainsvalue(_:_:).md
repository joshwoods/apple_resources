

- Core Foundation
-  CFSetContainsValue(\_:\_:) 

Function

# CFSetContainsValue(\_:\_:)

Returns a Boolean that indicates whether a set contains a given value.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFSetContainsValue(
    _ theSet: CFSet!,
    _ value: UnsafeRawPointer!
) -> Bool
```

## Parameters 

`theSet`  

The set to search.

`value`  

The value to match in `theSet`. Comparisons are made using the equal callback provided when `theSet` was created. If the equal callback was `NULL`, pointer equality (in C, ==) is used.

## Return Value

`true` if `value` is contained in `theSet`, otherwise `false`.

## Discussion

This function uses the equal callback. `value` and all elements in the set must be understood by the equal callback.

## See Also

### Examining a Set

func CFSetGetCount(CFSet!) -> CFIndex

Returns the number of values currently in a set.

func CFSetGetCountOfValue(CFSet!, UnsafeRawPointer!) -> CFIndex

Returns the number of values in a set that match a given value.

func CFSetGetValue(CFSet!, UnsafeRawPointer!) -> UnsafeRawPointer!

Obtains a specified value from a set.

func CFSetGetValueIfPresent(CFSet!, UnsafeRawPointer!, UnsafeMutablePointer&lt;UnsafeRawPointer?>!) -> Bool

Reports whether or not a value is in a set, and if it exists returns the value indirectly.

func CFSetGetValues(CFSet!, UnsafeMutablePointer&lt;UnsafeRawPointer?>!)

Obtains all values in a set.

