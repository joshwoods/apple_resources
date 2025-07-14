

- TVMLKit JS
- DataItem
-  identifier 

Instance Property

# identifier

A unique identifier for a data item provided by the associated JSON object.

tvOS 11.0+

``` source
readonly attribute String identifier;
```

## Discussion

The `identifier` property is mapped to the itemID attribute when the data item is converted to a DOM element. The underlying JSON objects being mapped must have a unique identifier for all JSON objects grouped under the same type.

## See Also

### Retrieving Data Item Information

type

The type for a data item provided by the associated JSON object.

