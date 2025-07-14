

- Create ML Components
- HumanBodyPoseExtractor
-  applied(to:eventHandler:) 

Instance Method

# applied(to:eventHandler:)

Extracts human body poses from a pixel buffer.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func applied(
    to image: CIImage,
    eventHandler: EventHandler? = nil
) async throws -> [Pose]
```

## Parameters 

`image`  

An image.

`eventHandler`  

An event handler.

## Return Value

A array of poses from all detected persons.

