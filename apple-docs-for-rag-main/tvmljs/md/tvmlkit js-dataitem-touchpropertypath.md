

- TVMLKit JS
- DataItem
-  touchPropertyPath 

Instance Method

# touchPropertyPath

Updates the property path.

tvOS 11.0+

``` source
void touchPropertyPath(
    in String path
);
```

## Parameters 

`path`  

The dot-separated sequence of properties from the receiver. The path can contain array indexers. For example, `items[0].title` refers to the `title` property stored in index location 0 in the `items` array.

## Discussion

The property path is explicitly updated, and all bound objects are notified.

## See Also

### Working with Property Paths

setPropertyPath

Sets the value associated with a property path.

getPropertyPath

Retrieves the value associated with a property path.

