

- AppKit
-  NSDockTilePlugIn 

Protocol

# NSDockTilePlugIn

A set of methods implemented by plug-ins that allow an app’s Dock tile to be customized while the app is not running.

macOS

``` source
protocol NSDockTilePlugIn : NSObjectProtocol
```

## Overview

Customizing an application’s Dock tile when the application itself is not running requires that you write a plug-in. The plug-in’s principal class must implement the NSDockTilePlugIn protocol.

The name of the plugin is indicated by a `NSDockTilePlugIn` key in the application’s `Info.plist` file.

The plugin is loaded in a system process at login time or when the application tile is added to the Dock. When the plugin is loaded, the principal class’ implementation of setDockTile(_:) is invoked, passing an NSDockTile for the plug-in to customize. If the principal class implements dockMenu() it is invoked whenever the user causes the application’s dock menu to be shown. When the dock tile is no longer valid (for example,. the application has been removed from the dock) -setDockTile(_:) is invoked with `nil`.

## Topics

### Setting the Dock Tile

func setDockTile(NSDockTile?)

Invoked when the plug-in is first loaded and when the application is removed from the Dock.

**Required**

### Getting the Dock Tile Menu

func dockMenu() -> NSMenu?

Invoked when the user causes the application’s dock menu to be shown.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### The Dock

class NSDockTile

The visual representation of your app’s miniaturized windows and app icon as they appear in the Dock.

