

- UIKit
- UIControl
-  performPrimaryAction() 

Instance Method

# performPrimaryAction()

Calls the method associated with the control’s primary action.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+tvOS 17.4+visionOS 1.1+

``` source
@MainActor
func performPrimaryAction()
```

## Discussion

This method invokes the primary action for the control, whether it’s a direct action, for example, a button tap, or presents further UI, for example, a contextual menu.

## See Also

### Triggering actions

func sendAction(UIAction)

func sendAction(Selector, to: Any?, for: UIEvent?)

Calls the specified action method.

func sendActions(for: UIControl.Event)

Calls the action methods associated with the specified events.

