

- CarPlay
- CPPointOfInterestTemplateDelegate
-  pointOfInterestTemplate(\_:didSelectPointOfInterest:) 

Instance Method

# pointOfInterestTemplate(\_:didSelectPointOfInterest:)

Tells the delegate when the user selects a point of interest.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+

``` source
optional func pointOfInterestTemplate(
    _ pointOfInterestTemplate: CPPointOfInterestTemplate,
    didSelectPointOfInterest pointOfInterest: CPPointOfInterest
)
```

## Parameters 

`pointOfInterestTemplate`  

The template that displays the map that contains the points of interest.

`pointOfInterest`  

The point of interest that the user selects.

## Discussion

CarPlay calls this method whenever the user selects a point of interest from the template’s map. The template displays a detail card for the selection, which contains secondary information and optional actions the user can perform.

Use the userInfo property to attach a value that provides additional context for the point of interest. You can then reference that value in your implementation of this method.

