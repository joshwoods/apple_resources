

- ManagedSettingsUI
- ShieldConfiguration
-  init(backgroundBlurStyle:backgroundColor:icon:title:subtitle:primaryButtonLabel:primaryButtonBackgroundColor:secondaryButtonLabel:) 

Initializer

# init(backgroundBlurStyle:backgroundColor:icon:title:subtitle:primaryButtonLabel:primaryButtonBackgroundColor:secondaryButtonLabel:)

Creates a shield configuration with the specified values.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
init(
    backgroundBlurStyle: UIBlurEffect.Style? = nil,
    backgroundColor: UIColor? = nil,
    icon: UIImage? = nil,
    title: ShieldConfiguration.Label? = nil,
    subtitle: ShieldConfiguration.Label? = nil,
    primaryButtonLabel: ShieldConfiguration.Label? = nil,
    primaryButtonBackgroundColor: UIColor? = nil,
    secondaryButtonLabel: ShieldConfiguration.Label? = nil
)
```

## Parameters 

`backgroundBlurStyle`  

A blur style to apply to the `backgroundColor`.

`backgroundColor`  

A color to display in the shield’s background.

`icon`  

An icon to display on the shield.

`title`  

A title for the shield.

`subtitle`  

Additional text to display on the shield.

`primaryButtonLabel`  

A label for the shield’s main button.

`primaryButtonBackgroundColor`  

A background color for the shield’s main button.

`secondaryButtonLabel`  

An additional button to display on the shield.

## Discussion

The system provides a default for any options that you don’t specify.

