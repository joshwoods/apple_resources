

- SpriteKit
- SKTileSet
-  init(from:) 

Initializer

# init(from:)

Initializes a tile set from a URL to an archived .sks file.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+watchOS 3.0+

``` source
convenience init?(from url: URL)
```

## Parameters 

`url`  

The URL of a tile set file.

## Return Value

A new tile set or `nil` if the URL doesn’t point to a valid tile set file.

## See Also

### Creating a Tile Set from a File

convenience init?(named: String)

Initializes a tile set by searching the app bundle for an archived `.sks` file by name.

