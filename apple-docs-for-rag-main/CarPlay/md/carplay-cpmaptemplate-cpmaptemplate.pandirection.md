

- CarPlay
- CPMapTemplate
-  CPMapTemplate.PanDirection 

Structure

# CPMapTemplate.PanDirection

The directions a user can pan (or move) a map displayed on the CarPlay screen.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
struct PanDirection
```

## Topics

### Pan Directions

static var down: CPMapTemplate.PanDirection

The user panned the map downward.

static var left: CPMapTemplate.PanDirection

The user panned the map to the left.

static var right: CPMapTemplate.PanDirection

The user panned the map to the right.

static var up: CPMapTemplate.PanDirection

The user panned the map upward.

### Initializers

init(rawValue: Int)

Initializes a pan direction using the specified raw value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Panning the Map

func mapTemplateDidShowPanningInterface(CPMapTemplate)

Tells the delegate that the panning interface is visible on the map.

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

func mapTemplate(CPMapTemplate, didEndPanGestureWithVelocity: CGPoint)

Tells the delegate that the pan gesture ended with the specified velocity.

func mapTemplate(CPMapTemplate, didUpdatePanGestureWithTranslation: CGPoint, velocity: CGPoint)

Tells the delegate that the pan gesture changed.

