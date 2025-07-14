

- SpriteKit
- SKTileSet
-  init(named:) 

Initializer

# init(named:)

Initializes a tile set by searching the app bundle for an archived `.sks` file by name.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
convenience init?(named name: String)
```

## Parameters 

`name`  

The name of the tile set to search for.

## Return Value

A new tile set or `nil` if a tile set with a matching name cannot be found.

## See Also

### Creating a Tile Set from a File

convenience init?(from: URL)

Initializes a tile set from a URL to an archived .sks file.

