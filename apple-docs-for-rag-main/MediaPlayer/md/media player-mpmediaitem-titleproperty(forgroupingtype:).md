

- Media Player
- MPMediaItem
-  titleProperty(forGroupingType:) 

Type Method

# titleProperty(forGroupingType:)

Obtains the title key for a specified grouping type.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
class func titleProperty(forGroupingType groupingType: MPMediaGrouping) -> String
```

## Parameters 

`groupingType`  

The grouping type that you want the title key for.

## Return Value

The title key for the group type.

## Discussion

Use this convenience method to obtain the key for the title that corresponds to a specified grouping type. For example, the following statement obtains the title key for the album grouping type:

- Swift
- Objective-C

```
let titleIDKey = [MPMediaItem.persistentIDProperty(forGroupingType: MPMediaGrouping.album)]
```

```
NSString *titleIDKey = [MPMediaItem titlePropertyForGroupingType: MPMediaGroupingAlbum];
```

You could then obtain the specific title that you want by using the value(forProperty:) method. MPMediaGrouping describes grouping keys.

## See Also

### Obtaining group properties

class func persistentIDProperty(forGroupingType: MPMediaGrouping) -> String

Obtains the persistent identifier key for a specified grouping type.

