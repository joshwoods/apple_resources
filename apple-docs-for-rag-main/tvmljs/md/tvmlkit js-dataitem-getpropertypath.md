

- TVMLKit JS
- DataItem
-  getPropertyPath 

Instance Method

# getPropertyPath

Retrieves the value associated with a property path.

tvOS 11.0+

``` source
Object getPropertyPath(
    in String path
);
```

## Parameters 

`path`  

The dot-separated sequence of properties from the receiver. The path can contain array indexers. For example, `items[0].title` refers to the `title` property stored in index location 0 in the `items` array.

## Return Value

The data item object contained in the path.

## See Also

### Working with Property Paths

setPropertyPath

Sets the value associated with a property path.

touchPropertyPath

Updates the property path.

