

- UIKit
- UITableView
-  UITableView.ScrollPosition 

Enumeration

# UITableView.ScrollPosition

The position in the table view (top, middle, bottom) to scroll a specified row to.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
enum ScrollPosition
```

## Overview

You set the scroll position through a parameter of the selectRow(at:animated:scrollPosition:), scrollToNearestSelectedRow(at:animated:), cellForRow(at:), and indexPathForSelectedRow methods.

## Topics

### Constants

case none

The table view scrolls the row of interest to be fully visible with a minimum of movement.

case top

The table view scrolls the row of interest to the top of the visible table view.

case middle

The table view scrolls the row of interest to the middle of the visible table view.

case bottom

The table view scrolls the row of interest to the bottom of the visible table view.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Scrolling the table view

func scrollToRow(at: IndexPath, at: UITableView.ScrollPosition, animated: Bool)

Scrolls through the table view until a row that an index path identifies is at a particular location on the screen.

func scrollToNearestSelectedRow(at: UITableView.ScrollPosition, animated: Bool)

Scrolls the table view so that the selected row nearest to a specified position in the table view is at that position.

