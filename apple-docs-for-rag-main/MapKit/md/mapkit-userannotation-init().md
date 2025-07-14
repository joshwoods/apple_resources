

- MapKit
- UserAnnotation
-  init() 

Initializer

# init()

Creates an annotation that displays the person’s current location.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
@MainActor @preconcurrency
init() where Content == DefaultUserAnnotationContent
```

## See Also

### Creating a user annotation

init(anchor: UnitPoint)

Creates an annotation that displays the person’s current location using the system styled user location indicator with the specified anchor point.

init(anchor: UnitPoint, content: (UserLocation) -> Content)

Creates an annotation that displays a person’s current location using the system styled user location indicator with the specified anchor point using a custom view.

init(anchor: UnitPoint, content: () -> Content)

Create an annotation that displays the person’s current location of the user using a custom view.

