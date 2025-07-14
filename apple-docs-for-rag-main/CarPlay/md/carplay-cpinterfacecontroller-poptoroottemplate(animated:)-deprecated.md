

- CarPlay
- CPInterfaceController
-  popToRootTemplate(animated:) Deprecated

Instance Method

# popToRootTemplate(animated:)

Pops all templates on the stack—except the root template—and updates the CarPlay display.

iOS 12.0–14.0DeprecatediPadOS 12.0–14.0DeprecatedMac Catalyst 13.1–14.0Deprecated

``` source
func popToRootTemplate(animated: Bool)
```

Deprecated

Use popToRootTemplate(animated:completion:) instead.

## Parameters 

`animated`  

A Boolean value that indicates whether the system animates the display of transitioning templates. Set to true to animate the transition.

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

func pop(to: CPTemplate, animated: Bool)

Pops templates until the specified template is at the top of the navigation stack.

Deprecated

func presentTemplate(CPTemplate, animated: Bool)

Presents a template modally.

Deprecated

func dismissTemplate(animated: Bool)

Dismisses the template that the interface controller is displaying modally.

Deprecated

