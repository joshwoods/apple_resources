

- CarPlay
- CPMapTemplateDelegate
-  mapTemplate(\_:startedTrip:using:) 

Instance Method

# mapTemplate(\_:startedTrip:using:)

Tells the delegate that the user selected a trip and route choice to navigate.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
optional func mapTemplate(
    _ mapTemplate: CPMapTemplate,
    startedTrip trip: CPTrip,
    using routeChoice: CPRouteChoice
)
```

## Parameters 

`mapTemplate`  

The current map template.

`trip`  

The selected trip.

`routeChoice`  

The selected route choice.

## See Also

### Handling Navigation Events

func mapTemplate(CPMapTemplate, selectedPreviewFor: CPTrip, using: CPRouteChoice)

Tells the delegate that the user selected a trip and route choice to preview.

func mapTemplateDidCancelNavigation(CPMapTemplate)

Tells the delegate that the system canceled the navigation.

func mapTemplateShouldProvideNavigationMetadata(CPMapTemplate) -> Bool

Asks the delegate whether the template should provide navigation metadata

