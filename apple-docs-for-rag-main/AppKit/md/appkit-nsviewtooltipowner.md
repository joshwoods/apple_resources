

- AppKit
-  NSViewToolTipOwner 

Protocol

# NSViewToolTipOwner

A set of methods for dynamically associating a tool tip with a view.

macOS

``` source
protocol NSViewToolTipOwner : NSObjectProtocol
```

## Overview

Tool tips are hints displayed to the user when the mouse hovers over a view. Adopt this protocol in views for which you want to provide tool tips. If the view does not implement this protocol, the system uses the description method instead.

## Topics

### Obtaining Tool Tip Strings

func view(NSView, stringForToolTip: NSView.ToolTipTag, point: NSPoint, userData: UnsafeMutableRawPointer?) -> String

Returns the tool tip string to be displayed due to the cursor pausing at location `point` within the tool tip rectangle identified by `tag` in the view `view`.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- NSForm
- NSMatrix
- NSTableHeaderView

