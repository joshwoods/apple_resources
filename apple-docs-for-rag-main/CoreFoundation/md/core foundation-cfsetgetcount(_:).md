

- Core Foundation
-  CFSetGetCount(\_:) 

Function

# CFSetGetCount(\_:)

Returns the number of values currently in a set.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
func CFSetGetCount(_ theSet: CFSet!) -> CFIndex
```

## Parameters 

`theSet`  

The set to examine.

## Return Value

The number of values in `theSet`.

## See Also

### Examining a Set

func CFSetContainsValue(CFSet!, UnsafeRawPointer!) -> Bool

Returns a Boolean that indicates whether a set contains a given value.

func CFSetGetCountOfValue(CFSet!, UnsafeRawPointer!) -> CFIndex

Returns the number of values in a set that match a given value.

func CFSetGetValue(CFSet!, UnsafeRawPointer!) -> UnsafeRawPointer!

Obtains a specified value from a set.

func CFSetGetValueIfPresent(CFSet!, UnsafeRawPointer!, UnsafeMutablePointer&lt;UnsafeRawPointer?>!) -> Bool

Reports whether or not a value is in a set, and if it exists returns the value indirectly.

func CFSetGetValues(CFSet!, UnsafeMutablePointer&lt;UnsafeRawPointer?>!)

Obtains all values in a set.

