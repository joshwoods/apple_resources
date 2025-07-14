

- MusicKit
-  ArtworkImage 

Structure

# ArtworkImage

A view that displays the image for a music item’s artwork.

MusicKitSwiftUIiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@MainActor @preconcurrency
struct ArtworkImage
```

## Overview

You can create an artwork image with an instance of Artwork.

While the artwork’s image data is loading, ArtworkImage automatically displays a placeholder with a solid color that matches the backgroundColor property of the artwork to render.

## Topics

### Initializers

init(Artwork, height: CGFloat)

Creates an instance with a specified height.

init(Artwork, width: CGFloat)

Creates an instance with a specified width.

init(Artwork, width: CGFloat, height: CGFloat)

Creates an instance with a specified width and height.

### Instance Properties

var body: some View

The content and behavior of the view.

### Type Aliases

typealias Body

The type of view representing the body of this view.

### Default Implementations

View Implementations

## Relationships

### Conforms To

- Sendable
- View

## See Also

### Artwork

struct Artwork

An object that represents artwork for a music item.

