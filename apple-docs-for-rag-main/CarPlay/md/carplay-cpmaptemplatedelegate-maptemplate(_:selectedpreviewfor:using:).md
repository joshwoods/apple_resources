

- CarPlay
- CPMapTemplateDelegate
-  mapTemplate(\_:selectedPreviewFor:using:) 

Instance Method

# mapTemplate(\_:selectedPreviewFor:using:)

Tells the delegate that the user selected a trip and route choice to preview.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
optional func mapTemplate(
    _ mapTemplate: CPMapTemplate,
    selectedPreviewFor trip: CPTrip,
    using routeChoice: CPRouteChoice
)
```

## Parameters 

`mapTemplate`  

The current map template.

`trip`  

The selected trip.

`routeChoice`  

The route chosen by the user.

## See Also

### Handling Navigation Events

func mapTemplate(CPMapTemplate, startedTrip: CPTrip, using: CPRouteChoice)

Tells the delegate that the user selected a trip and route choice to navigate.

func mapTemplateDidCancelNavigation(CPMapTemplate)

Tells the delegate that the system canceled the navigation.

func mapTemplateShouldProvideNavigationMetadata(CPMapTemplate) -> Bool

Asks the delegate whether the template should provide navigation metadata

