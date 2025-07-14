

- Core Foundation
-  CFSetGetValues(\_:\_:) 

Function

# CFSetGetValues(\_:\_:)

Obtains all values in a set.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFSetGetValues(
    _ theSet: CFSet!,
    _ values: UnsafeMutablePointer!
)
```

## Parameters 

`theSet`  

The set to examine.

`values`  

A C array of pointer-sized values to be filled with values from `theSet`. The value must be a valid C array of the appropriate type and of a size at least equal to the count of `theSet`). If the values are Core Foundation objects, ownership follows the The Create Rule.

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

func CFSetGetValueIfPresent(CFSet!, UnsafeRawPointer!, UnsafeMutablePointer&lt;UnsafeRawPointer?>!) -> Bool

Reports whether or not a value is in a set, and if it exists returns the value indirectly.

