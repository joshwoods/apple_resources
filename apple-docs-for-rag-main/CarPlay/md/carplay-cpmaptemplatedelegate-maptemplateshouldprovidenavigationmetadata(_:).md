

- CarPlay
- CPMapTemplateDelegate
-  mapTemplateShouldProvideNavigationMetadata(\_:) 

Instance Method

# mapTemplateShouldProvideNavigationMetadata(\_:)

Asks the delegate whether the template should provide navigation metadata

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+

``` source
optional func mapTemplateShouldProvideNavigationMetadata(_ mapTemplate: CPMapTemplate) -> Bool
```

## Parameters 

`mapTemplate`  

The current map template.

## Discussion

- Returns `true` if the template needs to provide navigation metadata, otherwise `false`.

## See Also

### Handling Navigation Events

func mapTemplate(CPMapTemplate, selectedPreviewFor: CPTrip, using: CPRouteChoice)

Tells the delegate that the user selected a trip and route choice to preview.

func mapTemplate(CPMapTemplate, startedTrip: CPTrip, using: CPRouteChoice)

Tells the delegate that the user selected a trip and route choice to navigate.

func mapTemplateDidCancelNavigation(CPMapTemplate)

Tells the delegate that the system canceled the navigation.

