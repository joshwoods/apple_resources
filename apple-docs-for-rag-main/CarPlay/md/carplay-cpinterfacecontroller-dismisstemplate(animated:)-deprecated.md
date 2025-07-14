

- CarPlay
- CPInterfaceController
-  dismissTemplate(animated:) Deprecated

Instance Method

# dismissTemplate(animated:)

Dismisses the template that the interface controller is displaying modally.

iOS 12.0–14.0DeprecatediPadOS 12.0–14.0DeprecatedMac Catalyst 13.1–14.0Deprecated

``` source
func dismissTemplate(animated: Bool)
```

Deprecated

Use dismissTemplate(animated:completion:) instead.

## Parameters 

`animated`  

A Boolean value that indicates whether the system animates the dismissal of the template. Set to true to animate the transition.

## Discussion

Calling this method when there’s no modal template displayed has no effect.

## See Also

### Deprecated Methods

func setRootTemplate(CPTemplate, animated: Bool)

Sets the root template, starting a new stack for the template navigation hierarchy.

Deprecated

func pushTemplate(CPTemplate, animated: Bool)

Pushes a template onto the navigation stack and updates the CarPlay display.

Deprecated

func popTemplate(animated: Bool)

Pops the top template from the navigation stack and updates the CarPlay display.

Deprecated

func popToRootTemplate(animated: Bool)

Pops all templates on the stack—except the root template—and updates the CarPlay display.

Deprecated

func pop(to: CPTemplate, animated: Bool)

Pops templates until the specified template is at the top of the navigation stack.

Deprecated

func presentTemplate(CPTemplate, animated: Bool)

Presents a template modally.

Deprecated

