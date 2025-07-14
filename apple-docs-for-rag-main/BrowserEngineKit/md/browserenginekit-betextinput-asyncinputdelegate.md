

- BrowserEngineKit
- BETextInput
-  asyncInputDelegate 

Instance Property

# asyncInputDelegate

A system-provided input delegate is assigned when the system is interested in input changes.

iOS 17.4+iPadOS 17.4+tvOS 17.4+visionOS 1.1+

``` source
weak var asyncInputDelegate: (any BETextInputDelegate)? { get set }
```

**Required**

## Mentioned in 

Integrating custom browser text views with UIKit

## Discussion

A delegate object that your text view notifies of events and changes in the text’s state.

## See Also

### Updating the text system

func canPerformAction(Selector, withSender: Any?) -> Bool

Returns whether text related actions, such those included in UIResponderStandardEditActions, can be handled

**Required**

