

- Media Player
- MPMediaItemArtwork
-  init(boundsSize:requestHandler:) 

Initializer

# init(boundsSize:requestHandler:)

Creates a new image from existing artwork with the specified bounds.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12.2+tvOS 10.0+visionOS 1.0+watchOS 5.0+

**macOS**

``` source
init(
    boundsSize: CGSize,
    requestHandler: @escaping (CGSize) -> NSImage
)
```

**iOS, iPadOS, Mac Catalyst, tvOS, visionOS, watchOS**

``` source
init(
    boundsSize: CGSize,
    requestHandler: @escaping (CGSize) -> UIImage
)
```

## Parameters 

`boundsSize`  

The original size of the artwork.

`requestHandler`  

A handler that the system calls for the requested artwork.

size  
The new size for the image.

## Return Value

The newly resized artwork.

## Discussion

The request handler returns the image in the newly requested size. The requested size must be less than the `boundsSize` parameter.

