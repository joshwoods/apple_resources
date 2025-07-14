

- Media Player
- MPMediaItemCollection
-  count 

Instance Property

# count

The number of media items in a collection.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var count: Int { get }
```

## Discussion

In some cases, using this property is more efficient than fetching the items array and asking for the count.

## See Also

### Using a media item collection

var items: [MPMediaItem]

The media items in a media item collection.

var representativeItem: MPMediaItem?

A media item whose properties are representative of the other media items in a collection.

var mediaTypes: MPMediaType

The types of the media items in a collection.

