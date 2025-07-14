

- ManagedSettingsUI
- ShieldConfiguration
-  secondaryButtonLabel 

Instance Property

# secondaryButtonLabel

The label of the optional secondary button.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
let secondaryButtonLabel: ShieldConfiguration.Label?
```

## Discussion

Unlike the primary button, this button is borderless and has no background. If this is `nil`, then the shield doesn’t have a secondary button.

## See Also

### Defining the Appearance

let backgroundBlurStyle: UIBlurEffect.Style?

A blur style to apply to the background of the shield.

let backgroundColor: UIColor?

A color for a shield to use in the background blur effect.

let icon: UIImage?

An icon to display in the center of the shield.

let primaryButtonBackgroundColor: UIColor?

The color to fill the contents of the rounded rectangle primary button.

let primaryButtonLabel: ShieldConfiguration.Label?

The label of the topmost rounded rectangle button.

let subtitle: ShieldConfiguration.Label?

The subtitle for a shield to display below the title.

let title: ShieldConfiguration.Label?

The title of the shield to display below the icon.

struct Label

The appearance of text labels within a shield.

