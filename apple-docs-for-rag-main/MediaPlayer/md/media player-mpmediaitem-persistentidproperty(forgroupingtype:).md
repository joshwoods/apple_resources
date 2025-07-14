

- Media Player
- MPMediaItem
-  persistentIDProperty(forGroupingType:) 

Type Method

# persistentIDProperty(forGroupingType:)

Obtains the persistent identifier key for a specified grouping type.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
class func persistentIDProperty(forGroupingType groupingType: MPMediaGrouping) -> String
```

## Parameters 

`groupingType`  

The grouping type that you want the persistent identifier key for.

## Return Value

The identifier for the group type.

## Discussion

Use this convenience method to obtain the key for a specific persistent identifier based on a grouping type. You can use that key, in turn, to obtain the value of a specific persistent ID of a media item, such as album title or artist name. Using this method simplifies such tasks as drilling down from an artist, to albums by that artist, to a specific album.

For example, the following statement returns the persistent identifier key for the album grouping type:

- Swift
- Objective-C

```
let albumIDKey = [MPMediaItem.persistentIDProperty(forGroupingType: MPMediaGrouping.album)]
```

```
```

You could then obtain the specific persistent ID that you want by using the value(forProperty:) method. MPMediaGrouping describes grouping keys.

## See Also

### Obtaining group properties

class func titleProperty(forGroupingType: MPMediaGrouping) -> String

Obtains the title key for a specified grouping type.

