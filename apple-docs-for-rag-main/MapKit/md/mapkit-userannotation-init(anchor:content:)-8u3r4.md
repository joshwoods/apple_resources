

- MapKit
- UserAnnotation
-  init(anchor:content:) 

Initializer

# init(anchor:content:)

Creates an annotation that displays a person’s current location using the system styled user location indicator with the specified anchor point using a custom view.

MapKitSwiftUIiOS 17.0+iPadOS 17.0+Mac CatalystmacOS 14.0+tvOS 17.0+visionOSwatchOS 10.0+

``` source
@MainActor @preconcurrency
init(
    anchor: UnitPoint = .center,
    @ViewBuilder content: @escaping (UserLocation) -> Content
)
```

## Parameters 

`anchor`  

A UnitPoint value that describes how to anchor the user location indicator to the person’s location. The default is center.

`content`  

The custom view to show at the person’s location.

## Return Value

Returns a UserAnnotation that displays a persons current location using the specified anchor location.

## See Also

### Creating a user annotation

init()

Creates an annotation that displays the person’s current location.

init(anchor: UnitPoint)

Creates an annotation that displays the person’s current location using the system styled user location indicator with the specified anchor point.

init(anchor: UnitPoint, content: () -> Content)

Create an annotation that displays the person’s current location of the user using a custom view.

