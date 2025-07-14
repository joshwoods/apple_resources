

- TVMLKit JS
- DataSource
- DataSource.DataSource
-  update 

Instance Method

# update

Updates an item in the data source array.

tvOS 13.0+

``` source
void update(
    in Array items, 
    in Array indexTitle, 
    in int segmentSize
);
```

## Discussion

The update API allows the existing data source to reuse already loaded items. This reduces any flashes that might traditionally occur in the UI because of these updates.

## See Also

### Modifying the Data Source

insert

Inserts a new item into the array.

delete

Deletes an item from the data source array.

move

Moves an item in the data source array.

replace

Replaces an item in the data source array.

