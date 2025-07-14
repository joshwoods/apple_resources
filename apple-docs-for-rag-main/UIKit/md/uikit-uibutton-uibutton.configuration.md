

- UIKit
- UIButton
-  UIButton.Configuration 

Structure

# UIButton.Configuration

A configuration that specifies the appearance and behavior of a button and its contents.

iOS 15.0+iPadOS 15.0+Mac CatalysttvOS 15.0+visionOS

``` source
struct Configuration
```

## Overview

You can configure and update a button with a UIButton.Configuration. A button configuration contains all the customization options available with other methods, such as setTitle(_:for:), and can serve as a replacement for those methods. Alternatively, you can use a configuration in combination with these other methods and adopt new button behaviors and appearance without rewriting your customized UIButton code.

## Topics

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

func updated(for: UIButton) -> UIButton.Configuration

Returns a copy of the configuration, updated for the given button.

### Configuring titles

var title: String?

The text of the title label the button displays.

var subtitle: String?

The text the subtitle label of the button displays.

var attributedTitle: AttributedString?

The text and style attributes for the button’s title label.

var attributedSubtitle: AttributedString?

The text and style attributes for the button’s subtitle label.

var titleTextAttributesTransformer: UIConfigurationTextAttributesTransformer?

A structure to update the attributed title when the button state changes.

var subtitleTextAttributesTransformer: UIConfigurationTextAttributesTransformer?

A structure to update the attributed subtitle when the button state changes.

struct UIConfigurationTextAttributesTransformer

Defines a text transformation that can affect the visual appearance of a string.

var titlePadding: CGFloat

The distance between the title and subtitle labels.

var titleAlignment: UIButton.Configuration.TitleAlignment

The text alignment the button uses to lay out the title and subtitle.

enum TitleAlignment

Specifies how to align a button’s title and subtitle.

var titleLineBreakMode: NSLineBreakMode

The line break mode the button uses to lay out the button’s title.

var subtitleLineBreakMode: NSLineBreakMode

The line break mode the button uses to lay out the button’s subtitle.

### Configuring images

var image: UIImage?

The foreground image the button displays.

var imagePadding: CGFloat

The distance between the button’s image and text.

var imagePlacement: NSDirectionalRectEdge

The edge against which the button places the image.

var imageReservation: CGFloat

A value that reserves space for the image in the same axis as the edge against which the button places the image.

var imageColorTransformer: UIConfigurationColorTransformer?

A block that transforms the image color when the button state changes.

var preferredSymbolConfigurationForImage: UIImage.SymbolConfiguration?

A requested configuration object for the button symbol image.

### Configuring layout

var buttonSize: UIButton.Configuration.Size

A size that requests a preferred size for the button.

enum Size

A predefined size for button elements.

var contentInsets: NSDirectionalEdgeInsets

The distance from the button’s content area to its bounds.

func setDefaultContentInsets()

Restores the default content insets.

### Configuring button colors

var baseBackgroundColor: UIColor?

The untransformed color for background views.

var baseForegroundColor: UIColor?

The untransformed color for foreground views.

### Configuring the button background

var background: UIBackgroundConfiguration

The configuration to customize the button background.

var cornerStyle: UIButton.Configuration.CornerStyle

The button style that controls the display behavior of the background corner radius.

enum CornerStyle

Settings that determine the appearance of the background corner radius.

### Configuring the indicator

var indicator: UIButton.Configuration.Indicator

The style of the indicator that appears on the button.

enum Indicator

Constants that determine the style of the indicator that appears on a button.

var indicatorColorTransformer: UIConfigurationColorTransformer?

The color transformer for resolving the indicator color.

### Configuring the activity indicator

var showsActivityIndicator: Bool

A Boolean value that determines whether the button displays an activity indicator instead of an image.

var activityIndicatorColorTransformer: UIConfigurationColorTransformer?

The color transformer for resolving the color of the activity indicator.

### Configuring selection behavior

var automaticallyUpdateForSelection: Bool

A Boolean value that determines whether the style automatically updates when the button is in a selected state.

### Configuring the appearance on macOS

var macIdiomStyle: UIButton.Configuration.MacIdiomStyle

The style to use when this button appears in macOS.

enum MacIdiomStyle

The button style your app uses when running in macOS.

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable

## See Also

### Creating buttons from a configuration object

convenience init(configuration: UIButton.Configuration, primaryAction: UIAction?)

Creates a new button with the specified configuration and registers the primary action event.

