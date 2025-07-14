

- ManagedSettingsUI
-  ShieldConfiguration 

Structure

# ShieldConfiguration

An object that defines the appearance of a shield to display over an application or website.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
struct ShieldConfiguration
```

## Overview

The system provides a default appearance for any properties you set to `nil`.

## Topics

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

let subtitle: ShieldConfiguration.Label?

The subtitle for a shield to display below the title.

let title: ShieldConfiguration.Label?

The title of the shield to display below the icon.

struct Label

The appearance of text labels within a shield.

### Creating the Shield Configuration

init(backgroundBlurStyle: UIBlurEffect.Style?, backgroundColor: UIColor?, icon: UIImage?, title: ShieldConfiguration.Label?, subtitle: ShieldConfiguration.Label?, primaryButtonLabel: ShieldConfiguration.Label?, primaryButtonBackgroundColor: UIColor?, secondaryButtonLabel: ShieldConfiguration.Label?)

Creates a shield configuration with the specified values.

## See Also

### Shield Configuration

class ShieldConfigurationDataSource

The base class for the principal object of an app extension that configures a shield’s appearance.

