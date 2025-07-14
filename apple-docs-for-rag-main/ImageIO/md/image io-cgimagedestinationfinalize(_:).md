

- Image I/O
-  CGImageDestinationFinalize(\_:) 

Function

# CGImageDestinationFinalize(\_:)

Writes image data and properties to the data, URL, or data consumer associated with the image destination.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.4+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func CGImageDestinationFinalize(_ idst: CGImageDestination) -> Bool
```

## Parameters 

`idst`  

An image destination.

## Return Value

`true` if the image destination successfully finalized the images, or `false` if an error occurred.

## Discussion

Call this method as the final step in saving your images. The output of the image destination isn’t valid until you call this method. After calling this function, you can’t add any more data to the image destination.

