

- CarPlay
- CPMapTemplateDelegate
-  mapTemplateDidCancelNavigation(\_:) 

Instance Method

# mapTemplateDidCancelNavigation(\_:)

Tells the delegate that the system canceled the navigation.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
optional func mapTemplateDidCancelNavigation(_ mapTemplate: CPMapTemplate)
```

## Parameters 

`mapTemplate`  

The current map template.

## See Also

### Handling Navigation Events

func mapTemplate(CPMapTemplate, selectedPreviewFor: CPTrip, using: CPRouteChoice)

Tells the delegate that the user selected a trip and route choice to preview.

func mapTemplate(CPMapTemplate, startedTrip: CPTrip, using: CPRouteChoice)

Tells the delegate that the user selected a trip and route choice to navigate.

func mapTemplateShouldProvideNavigationMetadata(CPMapTemplate) -> Bool

Asks the delegate whether the template should provide navigation metadata

