

- UIKit
- UITableView
-  sectionIndexMinimumDisplayRowCount 

Instance Property

# sectionIndexMinimumDisplayRowCount

The number of table rows at which to display the index list on the right edge of the table.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var sectionIndexMinimumDisplayRowCount: Int { get set }
```

## Discussion

This property is applicable only to table views in the UITableView.Style.plain style. The default value is zero.

## See Also

### Configuring the table index

var sectionIndexColor: UIColor?

The color to use for the table view’s index text.

var sectionIndexBackgroundColor: UIColor?

The color to use for the background of the table view’s section index.

var sectionIndexTrackingBackgroundColor: UIColor?

The color to use for the table view’s index background area.

class let indexSearch: String

A constant for adding the magnifying glass icon to the section index of a table view.

