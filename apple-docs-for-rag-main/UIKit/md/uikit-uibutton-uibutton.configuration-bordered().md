

- UIKit
- UIButton
- UIButton.Configuration
-  bordered() 

Type Method

# bordered()

Creates a configuration for a button that has a bordered style.

iOS 15.0+iPadOS 15.0+Mac CatalysttvOS 15.0+visionOS

``` source
static func bordered() -> UIButton.Configuration
```

## Return Value

A new configuration object.

## Discussion

This style provides an alternative name for the gray() style.

## See Also

### Creating configurations

static func plain() -> UIButton.Configuration

Creates a configuration for a button with a transparent background.

static func gray() -> UIButton.Configuration

Creates a configuration for a button with a gray background.

static func tinted() -> UIButton.Configuration

Creates a configuration for a button with a tinted background color.

static func filled() -> UIButton.Configuration

Creates a configuration for a button with a background filled with the button’s tint color.

static func borderless() -> UIButton.Configuration

Creates a configuration for a button that has a borderless style.

static func borderedTinted() -> UIButton.Configuration

Creates a configuration for a button that has a tinted, bordered style.

static func borderedProminent() -> UIButton.Configuration

Creates a configuration for a button that has a prominent, bordered style.

func updated(for: UIButton) -> UIButton.Configuration

Returns a copy of the configuration, updated for the given button.

