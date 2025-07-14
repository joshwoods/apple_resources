

- UIKit
- UIView
-  interactions 

Instance Property

# interactions

The array of interactions for the view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
var interactions: [any UIInteraction] { get set }
```

## Mentioned in 

Making a view into a drag source

Making a view into a drop destination

## See Also

### Adding and removing interactions

func addInteraction(any UIInteraction)

Adds an interaction to the view.

func removeInteraction(any UIInteraction)

Removes an interaction from the view.

protocol UIInteraction

The protocol that an interaction implements to access the view that owns it.

