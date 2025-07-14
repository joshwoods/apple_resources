

- Objective-C Runtime
- NSObject
-  imageUID() 

Instance Method

# imageUID()

Returns a unique string that identifies the data source item.

macOS

``` source
func imageUID() -> String!
```

## Return Value

The string that identifies the data source item

## Discussion

Your data source must implement this method. The image browser view uses this identifier to associate the data source item and its cache.

