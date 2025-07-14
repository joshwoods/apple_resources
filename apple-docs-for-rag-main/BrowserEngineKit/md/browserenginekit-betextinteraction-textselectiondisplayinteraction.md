

- BrowserEngineKit
- BETextInteraction
-  textSelectionDisplayInteraction 

Instance Property

# textSelectionDisplayInteraction

An interaction that manages the system’s text-selection UI.

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
@MainActor
var textSelectionDisplayInteraction: UITextSelectionDisplayInteraction { get }
```

## See Also

### Text selection

var delegate: (any BETextInteractionDelegate)?

A delegate object that the interaction notifies when the system changes the text selection.

protocol BETextInteractionDelegate

A set of methods that informs you about selection changes in text views.

func selectionBoundaryAdjusted(to: CGPoint, touchPhase: BESelectionTouchPhase, flags: BESelectionFlags)

Notifies the system after the text view adjusts its selection.

func selectionChangedWithGesture(at: CGPoint, gesture: BEGestureType, state: UIGestureRecognizer.State, flags: BESelectionFlags)

Notifies the system that the text view changed its selection.

