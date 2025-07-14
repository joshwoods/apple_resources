

- UIKit
- UITableView
-  contentHuggingElements 

Instance Property

# contentHuggingElements

A setting that determines which type of items tightly hug their content.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+tvOS 18.0+visionOS 2.0+

``` source
@MainActor
var contentHuggingElements: UITableViewContentHuggingElements { get set }
```

## Discussion

The default value of this property is sectionHeaders for plain-style table views in visionOS, and UITableViewContentHuggingElementsNone on all other platforms.

When the value of this property is sectionHeaders, header views tightly hug their content. This means header views don’t stretch to fill the width of the table view if its content’s intrinsic content size is less than the table view’s width.

## See Also

### Managing content-hugging behavior

struct UITableViewContentHuggingElements

Constants that determine which types of items in a table view tightly hug their content.

