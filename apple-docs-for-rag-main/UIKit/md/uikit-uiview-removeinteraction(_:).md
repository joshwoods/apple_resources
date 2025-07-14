

- UIKit
- UIView
-  removeInteraction(\_:) 

Instance Method

# removeInteraction(\_:)

Removes an interaction from the view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
func removeInteraction(_ interaction: any UIInteraction)
```

## Parameters 

`interaction`  

The interaction object to remove from the view.

## See Also

### Adding and removing interactions

func addInteraction(any UIInteraction)

Adds an interaction to the view.

var interactions: [any UIInteraction]

The array of interactions for the view.

protocol UIInteraction

The protocol that an interaction implements to access the view that owns it.

