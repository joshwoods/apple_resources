

- Core Foundation
-  CFSetGetValue(\_:\_:) 

Function

# CFSetGetValue(\_:\_:)

Obtains a specified value from a set.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFSetGetValue(
    _ theSet: CFSet!,
    _ value: UnsafeRawPointer!
) -> UnsafeRawPointer!
```

## Parameters 

`theSet`  

The set to examine.

`value`  

The value for which to search in `theSet`. Comparisons are made using the equal callback provided when `theSet` was created. If the equal callback was `NULL`, pointer equality (in C, ==) is used.

## Return Value

A pointer to the requested value, or `NULL` if the value is not in `theSet`. If the value is a Core Foundation object, Ownership follows the The Get Rule.

## Discussion

Since this function uses the equal callback, `value` all elements in the set must be understood by the equal callback. Depending on the implementation of the equal callback specified when creating `theSet`, the value returned may not have the same pointer equality as `value`.

## See Also

### Examining a Set

func CFSetContainsValue(CFSet!, UnsafeRawPointer!) -> Bool

Returns a Boolean that indicates whether a set contains a given value.

func CFSetGetCount(CFSet!) -> CFIndex

Returns the number of values currently in a set.

func CFSetGetCountOfValue(CFSet!, UnsafeRawPointer!) -> CFIndex

Returns the number of values in a set that match a given value.

func CFSetGetValueIfPresent(CFSet!, UnsafeRawPointer!, UnsafeMutablePointer&lt;UnsafeRawPointer?>!) -> Bool

Reports whether or not a value is in a set, and if it exists returns the value indirectly.

func CFSetGetValues(CFSet!, UnsafeMutablePointer&lt;UnsafeRawPointer?>!)

Obtains all values in a set.

