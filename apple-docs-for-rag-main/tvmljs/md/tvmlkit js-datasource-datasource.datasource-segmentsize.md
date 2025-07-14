

- TVMLKit JS
- DataSource
- DataSource.DataSource
-  segmentSize 

Instance Property

# segmentSize

The maximum number of indexes that are loaded each time the loadindexes event is triggered.

tvOS 13.0+

``` source
readonly attribute int segmentSize;
```

## Discussion

This property allows you to adjust the number of indexes to be loaded according to the capabilities of your server endpoints.

The `segmentSize` attribute defaults to 20 indexes.

## See Also

### Loading Elements

loadindexes

An event type that tells the data source to load its indexes.

