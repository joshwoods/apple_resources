

- Media Player
- MPMediaQuery
-  items 

Instance Property

# items

An array of media items that match the media query’s predicate.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var items: [MPMediaItem]? { get }
```

## Discussion

If no items match the predicate, this method returns an empty array. On error, returns `nil`.

## See Also

### Performing media queries

var collections: [MPMediaItemCollection]?

An array of media item collections whose contained items match the query’s media property predicate.

