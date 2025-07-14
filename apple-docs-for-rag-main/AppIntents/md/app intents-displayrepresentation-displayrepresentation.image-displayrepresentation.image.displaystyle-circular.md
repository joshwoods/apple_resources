

- App Intents
- DisplayRepresentation
- DisplayRepresentation.Image
- DisplayRepresentation.Image.DisplayStyle
-  circular 

Type Property

# circular

Display this representation in a circle.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
static var circular: DisplayRepresentation.Image.DisplayStyle { get }
```

## Discussion

Use this for situations where an entity is represented within your app as a circle, such as the colorful circles that are used to represent destinations in Apple Maps. When using this style, provide a full-bleed image, and the system will attempt to render your image within a circle mask when possible.

