

- UIKit
- UIButton
- UIButton.Configuration
-  updated(for:) 

Instance Method

# updated(for:)

Returns a copy of the configuration, updated for the given button.

iOS 15.0+iPadOS 15.0+Mac CatalysttvOS 15.0+visionOS

``` source
func updated(for button: UIButton) -> UIButton.Configuration
```

## Parameters 

`button`  

A button to use as a basis for the configuration.

## Return Value

An updated configuration. This method preserves custom values set on the configuration, and updates default values based on the button state.

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

static func bordered() -> UIButton.Configuration

Creates a configuration for a button that has a bordered style.

static func borderedTinted() -> UIButton.Configuration

Creates a configuration for a button that has a tinted, bordered style.

static func borderedProminent() -> UIButton.Configuration

Creates a configuration for a button that has a prominent, bordered style.

