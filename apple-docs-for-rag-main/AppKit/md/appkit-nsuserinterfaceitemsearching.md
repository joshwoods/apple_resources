

- AppKit
-  NSUserInterfaceItemSearching 

Protocol

# NSUserInterfaceItemSearching

A set of methods an app can implement to provide Spotlight for Help for its own custom help data.

macOS

``` source
protocol NSUserInterfaceItemSearching : NSObjectProtocol
```

## Overview

In general, users find the Help search functionality very useful. However, many large apps don’t use Apple Help API because of cross platform requirements, which means that some important Help topics are not presented as part of the Help menu. This API allows developers to incorporate their own Help topics and take full advantage of the Help feature.

In your app, you implement the NSUserInterfaceItemSearching protocol and then register your object with registerUserInterfaceItemSearchHandler(_:).

## Topics

### Show Help Menu

func localizedTitles(forItem: Any) -> [String]

Returns an array of localized strings that will form the help menu item.

**Required**

func showAllHelpTopics(forSearch: String)

If this method is implemented, a “Show All Help Topics” item will appear in the menu and this method is called when the user selects it.

### Search Help Content

func searchForItems(withSearch: String, resultLimit: Int, matchedItemHandler: ([Any]) -> Void)

Search for the specified items, with the result limit.

**Required**

func performAction(forItem: Any)

Invoked when the user selects a search result in Help menu.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### App Help

class NSHelpManager

An object for displaying online help for an app.

