

- TV Services
- TVContentIdentifier
-  container Deprecated

Instance Property

# container

The container that this content item is contained in.

tvOS 9.0–13.0Deprecated

``` source
@NSCopying
var container: TVContentIdentifier? { get }
```

Deprecated

TVContentIdentifier has been replaced by TVTopShelfContentProvider

## Discussion

Typically, this is the content identifier for the next larger grouping that this item is part of. For example, a podcast episode could be part of a larger podcast season, which could in turn be part of an entire podcast series. In this case, all three layers—episodes, seasons, and the series—would need their own unique identifiers.

The container value may be `nil`, in which case this item represents a top-level content item.

## See Also

### Inspecting an Identifier’s Contents

var identifier: String

The string that identifies this content item.

Deprecated

