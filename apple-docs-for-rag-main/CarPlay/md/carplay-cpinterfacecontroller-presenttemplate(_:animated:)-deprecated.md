

- CarPlay
- CPInterfaceController
-  presentTemplate(\_:animated:) Deprecated

Instance Method

# presentTemplate(\_:animated:)

Presents a template modally.

iOS 12.0–14.0DeprecatediPadOS 12.0–14.0DeprecatedMac Catalyst 13.1–14.0Deprecated

``` source
func presentTemplate(
    _ templateToPresent: CPTemplate,
    animated: Bool
)
```

Deprecated

Use presentTemplate(_:animated:completion:) instead.

## Parameters 

`templateToPresent`  

A template to display over currently displayed content on the CarPlay screen. The template must be one of the following types:

- CPActionSheetTemplate

- CPAlertTemplate

- CPVoiceControlTemplate

`animated`  

A Boolean value that indicates whether the system animates the display of transitioning templates. Set to true to animate the transition.

## Discussion

You can present only one template at a time.

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

func dismissTemplate(animated: Bool)

Dismisses the template that the interface controller is displaying modally.

Deprecated

