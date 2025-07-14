

- AppKit
- NSDockTilePlugIn
-  setDockTile(\_:) 

Instance Method

# setDockTile(\_:)

Invoked when the plug-in is first loaded and when the application is removed from the Dock.

macOS 10.5+

``` source
func setDockTile(_ dockTile: NSDockTile?)
```

**Required**

## Parameters 

`dockTile`  

The dock tile associated with the application, or `nil` if the application has been removed from the Dock.

## Discussion

The plugin is loaded in a system process at login time or when the application tile is added to the Dock.

The principal class of the plug-in must implement the `NSDockTilePlugIn` protocol.

