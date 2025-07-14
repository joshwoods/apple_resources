

- UIKit
- UIView
-  addInteraction(\_:) 

Instance Method

# addInteraction(\_:)

Adds an interaction to the view.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
func addInteraction(_ interaction: any UIInteraction)
```

## Parameters 

`interaction`  

The interaction object to add to the view.

## See Also

### Adding and removing interactions

func removeInteraction(any UIInteraction)

Removes an interaction from the view.

var interactions: [any UIInteraction]

The array of interactions for the view.

protocol UIInteraction

The protocol that an interaction implements to access the view that owns it.

