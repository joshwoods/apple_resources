

- UIKit
- UITableView
-  sectionIndexColor 

Instance Property

# sectionIndexColor

The color to use for the table view’s index text.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var sectionIndexColor: UIColor? { get set }
```

## Discussion

Table views can display an index along the side of the view, making it easier for users to navigate the contents of the table quickly. This property specifies the color to use for text displayed in this region. A value of `nil` represents the default color.

## See Also

### Configuring the table index

var sectionIndexMinimumDisplayRowCount: Int

The number of table rows at which to display the index list on the right edge of the table.

var sectionIndexBackgroundColor: UIColor?

The color to use for the background of the table view’s section index.

var sectionIndexTrackingBackgroundColor: UIColor?

The color to use for the table view’s index background area.

class let indexSearch: String

A constant for adding the magnifying glass icon to the section index of a table view.

