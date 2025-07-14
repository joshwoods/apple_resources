

- Device Management
- Dock
- Dock.StaticItem
-  Dock.StaticItem.Tile-data 

Device Management Profile

# Dock.StaticItem.Tile-data

The dictionary that contains details about a dock item.

macOS 10.7+Device Assignment ServicesVPP License Management

``` source
object Dock.StaticItem.Tile-data
```

## Properties

`file-data`

Dock.StaticItem.Tile-data.File-data

The data in a file. For Apple use only.

`file-type`

`integer`

 (Required) 

The type of tile:

- `0`: URL

- `1`: File

- `3`: Directory

Possible Values: `0, 1, 3`

`label`

`string`

 (Required) 

The label of the dock item.

`url`

`string`

The URL string.

## Topics

### Profiles

object Dock.StaticItem.Tile-data.File-data

For Apple use only.

## See Also

### Objects

object Dock.StaticItem

Items that are located on the Documents side of the Dock and cannot be removed from that location.

object Dock.StaticItem.Tile-data.File-data

For Apple use only.

