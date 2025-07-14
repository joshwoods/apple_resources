

- UIKit
- UIFontPickerViewController
-  init(configuration:) 

Initializer

# init(configuration:)

Creates a controller for a font picker view.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
init(configuration: UIFontPickerViewController.Configuration)
```

## Parameters 

`configuration`  

Settings for fonts the font picker should offer to the user and how to display those fonts.

## Return Value

A new view controller to show a font picker with the specified configuration.

## See Also

### Configuring a font picker to display in iOS

var configuration: UIFontPickerViewController.Configuration

Settings for fonts the font picker should offer to the user and how to display those fonts.

class Configuration

The filters and display settings a font picker view controller uses to set up a font picker.

