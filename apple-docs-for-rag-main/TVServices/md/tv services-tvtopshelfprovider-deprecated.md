

- TV Services
-  TVTopShelfProvider Deprecated

Protocol

# TVTopShelfProvider

The interface for providing items to display in the main menu’s Top Shelf user interface on an Apple TV.

tvOS 9.0–13.0Deprecated

``` source
protocol TVTopShelfProvider
```

Deprecated

TVTopShelfProvider has been replaced by TVTopShelfContentProvider

## Overview

You adopt this protocol in the principal class of your app’s TV Services extension. Apps that implement this extension can provide dynamic content to the Top Shelf element rather than having the system use the static image submitted with the app. The topShelfStyle property specifies the interface style you want, and the topShelfItems property specifies the content items to display. Whenever you change the content provided by the extension, post a TVTopShelfItemsDidChangeNotification notification to prompt the system to reload your content.

## Topics

### Implementing TV Services Extension Properties

var topShelfItems: [TVContentItem]

Returns an array of content items to be displayed.

**Required**

var topShelfStyle: TVTopShelfContentStyle

The user interface style that should be used to display the content items.

**Required**

enum TVTopShelfContentStyle

An enumerated type used to specify the style in which you want your content to be displayed.

### Notifying the System of Changes

static let TVTopShelfItemsDidChange: NSNotification.Name

A notification to post when your app’s Top Shelf content has changed.

