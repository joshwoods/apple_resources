

- UIKit
- UICollectionLayoutListConfiguration
-  contentHuggingElements 

Instance Property

# contentHuggingElements

A setting that determines which type of items tightly hug their content.

iOS 18.0+iPadOS 18.0+Mac CatalysttvOS 18.0+visionOS 2.0+

``` source
var contentHuggingElements: UICollectionLayoutListConfiguration.ContentHuggingElements { get set }
```

## Discussion

The default value of this property is supplementaryHeader in visionOS, and `[]` on all other platforms.

When the value of this property is supplementaryHeader, header views tightly hug their content. This means header views don’t stretch to fill the width of the collection view if its content’s intrinsic content size is less than the collection view’s width.

## See Also

### Managing content-hugging behavior

struct ContentHuggingElements

Constants that determine which types of items in a collection view tightly hug their content.

