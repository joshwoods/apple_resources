

- Foundation
- NSMapTable
-  dictionaryRepresentation() 

Instance Method

# dictionaryRepresentation()

Returns a dictionary representation of the map table.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func dictionaryRepresentation() -> [AnyHashable : ObjectType]
```

## Return Value

A dictionary representation of the map table.

## Discussion

The map table’s values and keys must conform to all the requirements specified in setObject(_:forKey:) in NSMutableDictionary.

