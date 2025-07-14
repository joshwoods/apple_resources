

- CarPlay
- CPInterfaceController
-  setRootTemplate(\_:animated:) Deprecated

Instance Method

# setRootTemplate(\_:animated:)

Sets the root template, starting a new stack for the template navigation hierarchy.

iOS 12.0–14.0DeprecatediPadOS 12.0–14.0DeprecatedMac Catalyst 13.1–14.0Deprecated

``` source
func setRootTemplate(
    _ rootTemplate: CPTemplate,
    animated: Bool
)
```

Deprecated

Use setRootTemplate(_:animated:completion:) instead.

## Parameters 

`rootTemplate`  

The root template. Replaces the current rootTemplate, if one exists.

`animated`  

Set to true to animate the presentation of the root template; ignored if there isn’t a current rootTemplate.

## See Also

### Deprecated Methods

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

func dismissTemplate(animated: Bool)

Dismisses the template that the interface controller is displaying modally.

Deprecated

