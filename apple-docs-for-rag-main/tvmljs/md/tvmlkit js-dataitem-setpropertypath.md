

- TVMLKit JS
- DataItem
-  setPropertyPath 

Instance Method

# setPropertyPath

Sets the value associated with a property path.

tvOS 11.0+

``` source
void setPropertyPath(
    in String path, 
    in Object value
);
```

## Parameters 

`path`  

The dot-separated sequence of properties from the receiver. The path can contain array indexers. For example, `items[0].title` refers to the `title` property stored in index location 0 in the `items` array.

`value`  

An object associated with the property path.

## Discussion

Set the property path to associate the data item objects contained in the `value` parameter with a section element. Listing 1 shows an example of data item objects contained in the `newItems` object added to the section that binds the `images` path; for example ``.

let section = shelf.getElementsByTagName(&quot;section&quot;).item(0)section.dataItem = new DataItem()

let newItems = results.map((result) => {
    let objectItem = new DataItem(result.type, result.ID);
    objectItem.url = result.url;
    return objectItem;
});

section.dataItem.setPropertyPath(&quot;images&quot;, newItems)

Listing 1 Setting the property path

## See Also

### Working with Property Paths

getPropertyPath

Retrieves the value associated with a property path.

touchPropertyPath

Updates the property path.

