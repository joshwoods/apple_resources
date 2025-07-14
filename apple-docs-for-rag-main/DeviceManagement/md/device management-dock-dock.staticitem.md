

- Device Management
- Dock
-  Dock.StaticItem 

Device Management Profile

# Dock.StaticItem

Items that are located on the Documents side of the Dock and cannot be removed from that location.

macOS 10.7+Device Assignment ServicesVPP License Management

``` source
object Dock.StaticItem
```

## Properties

`tile-data`

Dock.StaticItem.Tile-data

 (Required) 

The information about the dock item.

`tile-type`

`string`

 (Required) 

The type of tile.

Possible Values: `file-tile, directory-tile, url-tile`

## Topics

### Profiles

object Dock.StaticItem.Tile-data

The dictionary that contains details about a dock item.

## See Also

### Objects

object Dock.StaticItem.Tile-data

The dictionary that contains details about a dock item.

object Dock.StaticItem.Tile-data.File-data

For Apple use only.

