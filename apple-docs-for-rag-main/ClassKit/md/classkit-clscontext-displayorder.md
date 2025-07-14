

- ClassKit
- CLSContext
-  displayOrder 

Instance Property

# displayOrder

The position of a context relative to its siblings.

iOS 11.3+iPadOS 11.3+Mac Catalyst 11.3+macOS 11.0+visionOS 1.0+

``` source
var displayOrder: Int { get set }
```

## Mentioned in 

Building missing contexts

## Discussion

Setting this value provides a hint to the system about what order you intend sibling contexts to appear in. But this has nothing to do with the order in which a teacher assigns your content. Teachers are free to assign your content in any order they choose.

## See Also

### Managing context presentation

var topic: CLSContextTopic?

The area of study to which a context relates.

struct CLSContextTopic

The areas of study to which contexts may relate.

