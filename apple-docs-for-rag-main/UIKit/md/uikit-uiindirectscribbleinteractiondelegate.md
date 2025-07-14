

- UIKit
-  UIIndirectScribbleInteractionDelegate 

Protocol

# UIIndirectScribbleInteractionDelegate

Methods that customize behavior on views that aren’t formally text input views.

iOS 14.0+iPadOS 14.0+Mac CatalystvisionOS

``` source
protocol UIIndirectScribbleInteractionDelegate : NSObjectProtocol
```

## Topics

### Identifying Elements

associatedtype ElementIdentifier : Hashable = String

A unique identifier for a control that isn’t a text field in a Scribble interaction.

**Required**

### Managing Focus

func indirectScribbleInteraction(any UIInteraction, isElementFocused: Self.ElementIdentifier) -> Bool

Asks the delegate if an element is currently focused, according to the internal state of the interaction’s view.

**Required**

func indirectScribbleInteraction(any UIInteraction, focusElementIfNeeded: Self.ElementIdentifier, referencePoint: CGPoint, completion: ((any UIResponder &amp; UITextInput)?) -> Void)

Asks the delegate to focus an element to handle text edits.

**Required**

func indirectScribbleInteraction(any UIInteraction, shouldDelayFocusForElement: Self.ElementIdentifier) -> Bool

Allow the delegate to delay focusing an element.

**Required** Default implementation provided.

### Tracking Scribble Input

func indirectScribbleInteraction(any UIInteraction, willBeginWritingInElement: Self.ElementIdentifier)

Informs the delegate when the user begins writing.

**Required** Default implementation provided.

func indirectScribbleInteraction(any UIInteraction, didFinishWritingInElement: Self.ElementIdentifier)

Informs the delegate when the user finishes writing.

**Required** Default implementation provided.

### Finding Elements and Frames

func indirectScribbleInteraction(any UIInteraction, frameForElement: Self.ElementIdentifier) -> CGRect

Asks the delegate to provide the frame of an element.

**Required**

func indirectScribbleInteraction(any UIInteraction, requestElementsIn: CGRect, completion: ([Self.ElementIdentifier]) -> Void)

Asks the delegate to return the locations of text input elements inside the specified rectangle of the view.

**Required**

### Instance Methods

func indirectScribbleInteraction(any UIInteraction, focusElementIfNeeded: Self.ElementIdentifier, referencePoint: CGPoint) async -> (any UIResponder &amp; UITextInput)?

**Required** Default implementation provided.

func indirectScribbleInteraction(any UIInteraction, requestElementsIn: CGRect) async -> [Self.ElementIdentifier]

**Required** Default implementation provided.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Custom views

class UIIndirectScribbleInteraction

An interaction for using Scribble to enter text by writing on a view that isn’t formally a text input.

associatedtype ElementIdentifier : Hashable = String

A unique identifier for a control that isn’t a text field in a Scribble interaction.

**Required**

