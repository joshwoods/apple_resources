

- Create ML Components
- ImageReader
-  applied(to:eventHandler:) 

Instance Method

# applied(to:eventHandler:)

Reads an image URL as a `CIImage`.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func applied(
    to url: URL,
    eventHandler: EventHandler? = nil
) throws -> CIImage
```

## Parameters 

`url`  

A image URL.

`eventHandler`  

An event handler.

## Return Value

An image.

