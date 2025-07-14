

- UIKit
-  UINavigationItemRenameDelegate 

Protocol

# UINavigationItemRenameDelegate

Methods an object implements to rename a navigation item.

iOS 16.0+iPadOS 16.0+Mac CatalystvisionOS

``` source
@MainActor @preconcurrency
protocol UINavigationItemRenameDelegate : AnyObject
```

## Overview

A navigation item (UINavigationItem) uses this delegate to determine whether a person can change the navigation item’s title and to handle the rename process.

Related Sessions from WWDC22

Session 10069: Meet desktop-class iPad

Session 10070: Build a desktop-class iPad app

## Topics

### Determining rename support

func navigationItemShouldBeginRenaming(UINavigationItem) -> Bool

Asks the delegate whether the navigation item supports renaming.

**Required** Default implementation provided.

func navigationItem(UINavigationItem, shouldEndRenamingWith: String) -> Bool

Asks the delegate whether to continue or abandon the rename process.

**Required** Default implementation provided.

### Handling the rename process

func navigationItem(UINavigationItem, willBeginRenamingWith: String, selectedRange: Range&lt;String.Index>) -> (String, Range&lt;String.Index>)

Tells the delegate when the rename process starts.

**Required** Default implementation provided.

func navigationItem(UINavigationItem, didEndRenamingWith: String)

Tells the delegate when the rename process ends.

**Required**

## See Also

### Renaming documents

var renameDelegate: (any UINavigationItemRenameDelegate)?

The delegate for renaming the navigation item.

