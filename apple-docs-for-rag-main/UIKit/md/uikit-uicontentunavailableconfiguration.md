

- UIKit
-  UIContentUnavailableConfiguration 

Structure

# UIContentUnavailableConfiguration

A content configuration for a content-unavailable view.

iOS 17.0+iPadOS 17.0+Mac CatalysttvOS 17.0+visionOS

``` source
struct UIContentUnavailableConfiguration
```

## Overview

A content-unavailable configuration is a composable description of a view that indicates your app can’t display content. Using a content-unavailable configuration, you can obtain system default styling for a variety of different empty states. Fill the configuration with placeholder content, and then assign it to a view controller’s contentUnavailableConfiguration, or to a UIContentUnavailableView.

The following screenshot shows an example of a content-unavailable view configured by setting the image, text, and secondaryText properties.

## Topics

### Structures

struct ButtonProperties

Properties to configure buttons for a content-unavailable view.

struct ImageProperties

Properties to configure the image for a content-unavailable view.

struct TextProperties

Properties to configure text for a content-unavailable view.

### Instance Properties

var alignment: UIContentUnavailableConfiguration.Alignment

The alignment of the image, text, and buttons.

var attributedText: NSAttributedString?

An attributed variant of the primary text.

var axesPreservingSuperviewLayoutMargins: UIAxis

Configures which margins use the layout margins inherited from the superview.

var background: UIBackgroundConfiguration

The configuration for the background.

var button: UIButton.Configuration

The configuration for the primary button.

var buttonProperties: UIContentUnavailableConfiguration.ButtonProperties

Additional configuration for the primary button.

var buttonToSecondaryButtonPadding: CGFloat

The padding between the primary button and secondary button.

var directionalLayoutMargins: NSDirectionalEdgeInsets

The margins between the content and the edges of the content view.

var image: UIImage?

The image to display.

var imageProperties: UIContentUnavailableConfiguration.ImageProperties

The configuration for the image.

var imageToTextPadding: CGFloat

The padding between the image and the primary text.

var secondaryAttributedText: NSAttributedString?

An attributed variant of the secondary text.

var secondaryButton: UIButton.Configuration

The configuration for the secondary button.

var secondaryButtonProperties: UIContentUnavailableConfiguration.ButtonProperties

Additional configuration for the secondary button.

var secondaryText: String?

The secondary text to display.

var secondaryTextProperties: UIContentUnavailableConfiguration.TextProperties

Properties for configuring the secondary text.

var text: String?

The primary text to display.

var textProperties: UIContentUnavailableConfiguration.TextProperties

Properties for configuring the primary text.

var textToButtonPadding: CGFloat

The padding between the text and buttons.

var textToSecondaryTextPadding: CGFloat

The padding between the primary and secondary text.

### Type Methods

static func empty() -> UIContentUnavailableConfiguration

Creates the default configuration for unavailable content.

static func loading() -> UIContentUnavailableConfiguration

Creates the default configuration for content that’s loading.

static func search() -> UIContentUnavailableConfiguration

Creates the default configuration for searches that return no results.

### Enumerations

enum Alignment

Constants to define the alignment of views in a content-unavailable view.

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomReflectable
- CustomStringConvertible
- Equatable
- Hashable
- UIContentConfiguration

## See Also

### Unavailable content configurations

struct UIContentUnavailableConfigurationState

A structure that encapsulates state for a content-unavailable view.

