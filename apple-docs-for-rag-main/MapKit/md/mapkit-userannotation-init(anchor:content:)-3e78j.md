

- MapKit
- UserAnnotation
-  init(anchor:content:) 

Initializer

# init(anchor:content:)

Create an annotation that displays the person’s current location of the user using a custom view.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
@MainActor @preconcurrency
init(
    anchor: UnitPoint = .center,
    @ViewBuilder content: @escaping () -> Content
)
```

## Parameters 

`anchor`  

How to anchor the user location indicator around the person’s location. The default is center.

`content`  

The custom view used to indicate the person’s location.

## See Also

### Creating a user annotation

init()

Creates an annotation that displays the person’s current location.

init(anchor: UnitPoint)

Creates an annotation that displays the person’s current location using the system styled user location indicator with the specified anchor point.

init(anchor: UnitPoint, content: (UserLocation) -> Content)

Creates an annotation that displays a person’s current location using the system styled user location indicator with the specified anchor point using a custom view.

