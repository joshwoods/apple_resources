

- AppKit
-  NSTextFinderBarContainer 

Protocol

# NSTextFinderBarContainer

A protocol that provides a container in which the find bar is displayed.

macOS

``` source
protocol NSTextFinderBarContainer : NSObjectProtocol
```

## Overview

To display the find bar, a container for the find bar must be specified. You specify a find bar container using the findBarContainer of the NSTextFinder class.

See NSTextFinder for more information.

## Topics

### Find Bar View

var findBarView: NSView?

The view assigned by the text bar as the find bar view for the container.

**Required**

func contentView() -> NSView?

A view hierarchy that contains all the views which display the contents being searched.

var isFindBarVisible: Bool

Returns whether the container should display its find bar.

**Required**

### Find Bar Height

func findBarViewDidChangeHeight()

Notifies the find bar container that the find bar has changed its height.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

### Conforming Types

- NSScrollView

## See Also

### Search and Replace

class NSTextFinder

An optional search-and-replace find interface inside a view, usually a scroll view.

protocol NSTextFinderClient

A set of methods implemented by objects that support searching using the NSTextFinder class and the in-window text find bar.

