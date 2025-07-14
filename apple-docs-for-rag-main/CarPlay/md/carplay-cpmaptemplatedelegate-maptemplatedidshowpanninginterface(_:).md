

- CarPlay
- CPMapTemplateDelegate
-  mapTemplateDidShowPanningInterface(\_:) 

Instance Method

# mapTemplateDidShowPanningInterface(\_:)

Tells the delegate that the panning interface is visible on the map.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
optional func mapTemplateDidShowPanningInterface(_ mapTemplate: CPMapTemplate)
```

## Parameters 

`mapTemplate`  

The current map template.

## See Also

### Panning the Map

func mapTemplateWillDismissPanningInterface(CPMapTemplate)

Tells the delegate that the panning interface will disappear from the map.

func mapTemplateDidDismissPanningInterface(CPMapTemplate)

Tells the delegate that the panning interface is no longer visible on the map.

func mapTemplateDidBeginPanGesture(CPMapTemplate)

Tells the delegate that the pan gesture has started.

func mapTemplate(CPMapTemplate, panBeganWith: CPMapTemplate.PanDirection)

Tells the delegate that the user is starting to pan the map.

func mapTemplate(CPMapTemplate, panWith: CPMapTemplate.PanDirection)

Tells the delegate that the user is panning in a certain direction on the map.

func mapTemplate(CPMapTemplate, panEndedWith: CPMapTemplate.PanDirection)

Tells the delegate that the user stopped panning the map.

struct PanDirection

The directions a user can pan (or move) a map displayed on the CarPlay screen.

func mapTemplate(CPMapTemplate, didEndPanGestureWithVelocity: CGPoint)

Tells the delegate that the pan gesture ended with the specified velocity.

func mapTemplate(CPMapTemplate, didUpdatePanGestureWithTranslation: CGPoint, velocity: CGPoint)

Tells the delegate that the pan gesture changed.

