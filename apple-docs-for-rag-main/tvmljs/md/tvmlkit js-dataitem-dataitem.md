

- TVMLKit JS
- DataItem
-  DataItem 

Instance Method

# DataItem

Creates a new data item.

tvOS 11.0+

``` source
new DataItem(
    in String type, 
    in String identifier
);
```

## Parameters 

`type`  

The group identifier that associates the data item to a prototype attribute.

`identifier`  

A unique identifier for the data item.

## Discussion

Each data item in the same type group must have a unique identifier. Assign any other JSON object keys to the data item after it has been created. Listing 1 shows JSON objects being mapped to data items. The `url` and `title` keys and values are added to each data item after creation.

let newItems = results.map((result) => {
    let objectItem = new DataItem(result.type, result.ID);
    objectItem.url = result.url;
    objectItem.title = result.title;
    return objectItem;
});

Listing 1 Mapping JSON objects to data items

