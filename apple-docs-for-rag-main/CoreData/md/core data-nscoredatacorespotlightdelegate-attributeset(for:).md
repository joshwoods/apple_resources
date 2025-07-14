

- Core Data
- NSCoreDataCoreSpotlightDelegate
-  attributeSet(for:) 

Instance Method

# attributeSet(for:)

Returns the searchable attributes for the specified managed object.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+visionOS 1.0+

``` source
func attributeSet(for object: NSManagedObject) -> CSSearchableItemAttributeSet?
```

## Parameters 

`object`  

The managed object to index.

## Return Value

An instance of CSSearchableItemAttributeSet that provides the searchable item’s attributes.

## Discussion

Important

If you enable isIndexedBySpotlight on a property description that describes a relationship, override this method and return the necessary set of attributes. Core Data doesn’t automatically infer indexable information for relationships.

To prevent Core Spotlight from indexing a specific managed object, override this method and return `nil` for that object.

## See Also

### Managing the Index

func deleteSpotlightIndex(completionHandler: ((any Error)?) -> Void)

Deletes all searchable items from the configured index.

func startSpotlightIndexing()

Starts the indexing of the store’s entities.

func stopSpotlightIndexing()

Stops the indexing of the store’s entities.

