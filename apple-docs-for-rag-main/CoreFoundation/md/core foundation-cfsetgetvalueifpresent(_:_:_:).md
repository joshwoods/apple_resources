

- Core Foundation
-  CFSetGetValueIfPresent(\_:\_:\_:) 

Function

# CFSetGetValueIfPresent(\_:\_:\_:)

Reports whether or not a value is in a set, and if it exists returns the value indirectly.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFSetGetValueIfPresent(
    _ theSet: CFSet!,
    _ candidate: UnsafeRawPointer!,
    _ value: UnsafeMutablePointer!
) -> Bool
```

## Parameters 

`theSet`  

The set to examine.

`candidate`  

The value for which to search in `theSet`. Comparisons are made using the equal callback provided when `theSet` was created. If the equal callback was `NULL`, pointer equality (in C, ==) is used.

`value`  

Upon return contains the matching value if it exists in `theSet`, otherwise `NULL`. If the value is a Core Foundation object, ownership follows the The Get Rule.

## Return Value

`true` if `value` exists in `theSet`, otherwise `false`.

## Discussion

This function uses the equal callback. `candidate` and all elements in the set must be understood by the equal callback. Depending on the implementation of the equal callback specified when creating `theSet`, the value returned in `value` may not have the same pointer equality as `candidate`.

## See Also

### Examining a Set

func CFSetContainsValue(CFSet!, UnsafeRawPointer!) -> Bool

Returns a Boolean that indicates whether a set contains a given value.

func CFSetGetCount(CFSet!) -> CFIndex

Returns the number of values currently in a set.

func CFSetGetCountOfValue(CFSet!, UnsafeRawPointer!) -> CFIndex

Returns the number of values in a set that match a given value.

func CFSetGetValue(CFSet!, UnsafeRawPointer!) -> UnsafeRawPointer!

Obtains a specified value from a set.

func CFSetGetValues(CFSet!, UnsafeMutablePointer&lt;UnsafeRawPointer?>!)

Obtains all values in a set.

