

- TVMLKit JS
- DataSource
- DataSource.DataSource
-  loadindexes 

Instance Property

# loadindexes

An event type that tells the data source to load its indexes.

tvOS 13.0+

``` source
attribute  loadindexes;
```

## Discussion

This event gets triggered when TVMLKit recognizes that the `DataSource` needs to load more indexes. TVMLKit invokes the event when there are visible cells onscreen consisting of incomplete data segments. For example, when the `DataSource` is set up to support lazy loading of data and it begins to request uninitialized objects, this event is triggered.

The `loadIndexes` event contains its `DataSource `objectas the target, as well as a `request` property, which is a LoadIndexesRequest object.

## See Also

### Loading Elements

segmentSize

The maximum number of indexes that are loaded each time the loadindexes event is triggered.

