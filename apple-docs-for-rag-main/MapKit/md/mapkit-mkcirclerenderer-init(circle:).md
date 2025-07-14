

- MapKit
- MKCircleRenderer
-  init(circle:) 

Initializer

# init(circle:)

Creates a new overlay view using the specified circle overlay object.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.2+visionOS 1.0+

``` source
init(circle: MKCircle)
```

## Parameters 

`circle`  

The circle overlay containing the information about the circular area for the renderer to draw. The renderer maintains a strong reference to the object you provide. This parameter can’t be `nil`.

## Return Value

An initialized circle renderer object.

