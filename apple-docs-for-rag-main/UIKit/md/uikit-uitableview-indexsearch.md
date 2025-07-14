

- UIKit
- UITableView
-  indexSearch 

Type Property

# indexSearch

A constant for adding the magnifying glass icon to the section index of a table view.

iOS 3.0+iPadOS 3.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class let indexSearch: String
```

## Discussion

If the data source includes this constant string in the array of strings it returns in sectionIndexTitles(for:), the section index displays a magnifying glass icon at the corresponding index location. This location should generally be the first title in the index.

## See Also

### Configuring the table index

var sectionIndexMinimumDisplayRowCount: Int

The number of table rows at which to display the index list on the right edge of the table.

var sectionIndexColor: UIColor?

The color to use for the table view’s index text.

var sectionIndexBackgroundColor: UIColor?

The color to use for the background of the table view’s section index.

var sectionIndexTrackingBackgroundColor: UIColor?

The color to use for the table view’s index background area.

