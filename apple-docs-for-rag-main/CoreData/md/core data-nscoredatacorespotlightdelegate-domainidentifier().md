

- Core Data
- NSCoreDataCoreSpotlightDelegate
-  domainIdentifier() 

Instance Method

# domainIdentifier()

Returns the domain identifier.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+

``` source
func domainIdentifier() -> String
```

## Discussion

The default value is the persistent store’s identifier.

## See Also

### Configuring the Index

var isIndexingEnabled: Bool

A Boolean value that indicates whether Core Data is currently updating the Core Spotlight index with the persistent store’s entities.

func indexName() -> String?

Returns the index’s name.

