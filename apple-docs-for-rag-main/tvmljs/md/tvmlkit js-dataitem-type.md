

- TVMLKit JS
- DataItem
-  type 

Instance Property

# type

The type for a data item provided by the associated JSON object.

tvOS 11.0+

``` source
readonly attribute String type;
```

## Discussion

When the data item is converted to a DOM element, this property maps a data item to a prototype attribute. For example, `` associates all data items with the artwork type to the lockup element.

## See Also

### Retrieving Data Item Information

identifier

A unique identifier for a data item provided by the associated JSON object.

