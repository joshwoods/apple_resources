

- CarPlay
- CPInterfaceController
-  pushTemplate(\_:animated:) Deprecated

Instance Method

# pushTemplate(\_:animated:)

Pushes a template onto the navigation stack and updates the CarPlay display.

iOS 12.0–14.0DeprecatediPadOS 12.0–14.0DeprecatedMac Catalyst 13.1–14.0Deprecated

``` source
func pushTemplate(
    _ templateToPush: CPTemplate,
    animated: Bool
)
```

Deprecated

Use pushTemplate(_:animated:completion:) instead.

## Parameters 

`templateToPush`  

The template to push onto the navigation stack.

`animated`  

Set to true to animate the presentation of the template.

## See Also

### Deprecated Methods

func setRootTemplate(CPTemplate, animated: Bool)

Sets the root template, starting a new stack for the template navigation hierarchy.

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

