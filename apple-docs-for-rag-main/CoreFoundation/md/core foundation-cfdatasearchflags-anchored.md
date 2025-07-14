

- Core Foundation
- CFDataSearchFlags
-  anchored 

Type Property

# anchored

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var anchored: CFDataSearchFlags { get }
```

## Discussion

Performs searching only on bytes at the beginning or, if `kCFDataSearchBackwards` is also specified, at the end of the search range. No match at the beginning or end means nothing is found, even if a matching sequence of bytes occurs elsewhere in the data object.

## See Also

### Constants

static var backwards: CFDataSearchFlags

