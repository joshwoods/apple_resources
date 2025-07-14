

- Media Player
- MPMusicPlayerStoreQueueDescriptor
-  startItemID 

Instance Property

# startItemID

The item identified by the store identifier to play first.

iOS 10.1+iPadOS 10.1+Mac Catalyst 13.1+tvOS 14.0+visionOS 1.0+

``` source
var startItemID: String? { get set }
```

## Discussion

When this property isn’t set, the value is nil and the first item in the queue is the first item to play.

## See Also

### Store identifier queue descriptor properties

var storeIDs: [String]?

An array containing the store identifiers found by the query used to create the queue descriptor.

