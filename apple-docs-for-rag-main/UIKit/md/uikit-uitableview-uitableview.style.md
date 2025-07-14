

- UIKit
- UITableView
-  UITableView.Style 

Enumeration

# UITableView.Style

Constants for the table view styles.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
enum Style
```

## Overview

You set the table style when you initialize the table view (see init(frame:style:)). You can’t modify the style thereafter.

## Topics

### Styles

case plain

A plain table view.

case grouped

A table view where sections have distinct groups of rows.

case insetGrouped

A table view where the grouped sections are inset with rounded corners.

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

### Configuring the table’s appearance

var style: UITableView.Style

The style of the table view.

var tableHeaderView: UIView?

The view that displays above the table’s content.

var tableFooterView: UIView?

The view that displays below the table’s content.

var backgroundView: UIView?

The background view of the table view.

