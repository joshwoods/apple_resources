

- ManagedSettingsUI
- ShieldConfiguration
-  subtitle 

Instance Property

# subtitle

The subtitle for a shield to display below the title.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
let subtitle: ShieldConfiguration.Label?
```

## Discussion

Use a `subtitle` to provide more information, such as the reason for shielding the content.

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

let secondaryButtonLabel: ShieldConfiguration.Label?

The label of the optional secondary button.

let title: ShieldConfiguration.Label?

The title of the shield to display below the icon.

struct Label

The appearance of text labels within a shield.

