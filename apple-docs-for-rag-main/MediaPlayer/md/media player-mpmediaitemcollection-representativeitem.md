

- Media Player
- MPMediaItemCollection
-  representativeItem 

Instance Property

# representativeItem

A media item whose properties are representative of the other media items in a collection.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var representativeItem: MPMediaItem? { get }
```

## Discussion

The media items in a collection typically share common property values, owing to how you built the collection. For example, if you build a collection based on a predicate that uses the MPMediaItemPropertyArtist property, all items in the collection share the same artist name. You can use the `representativeItem` property to efficiently obtain values for such common properties—often more efficiently than fetching an item from the items array.

## See Also

### Using a media item collection

var items: [MPMediaItem]

The media items in a media item collection.

var count: Int

The number of media items in a collection.

var mediaTypes: MPMediaType

The types of the media items in a collection.

