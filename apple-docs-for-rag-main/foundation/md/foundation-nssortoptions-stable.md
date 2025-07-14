

- Foundation
- NSSortOptions
-  stable 

Type Property

# stable

Specifies that the sorted results should return compared items having equal value in the order they occurred originally.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var stable: NSSortOptions { get }
```

## Discussion

If this option is unspecified, equal objects may, or may not be returned in their original order.

## See Also

### Constants

static var concurrent: NSSortOptions

Specifies that the Block sort operation should be concurrent.

