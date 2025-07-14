

- Safari Services
- SFSafariViewController
-  SFSafariViewController.Configuration 

Class

# SFSafariViewController.Configuration

A configuration object that defines how a Safari view controller should be initialized.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
class Configuration
```

## Overview

Use a configuration object with the init(url:configuration:) method to initialize your view controller.

## Topics

### Configuring a Safari View Controller

var entersReaderIfAvailable: Bool

A value that specifies whether Safari should enter Reader mode, if it is available.

var barCollapsingEnabled: Bool

var eventAttribution: UIEventAttribution?

An object you use to send tap event attribution data to the browser for Private Click Measurement.

### Instance Properties

var activityButton: SFSafariViewController.ActivityButton?

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Creating a View Controller

init(url: URL, configuration: SFSafariViewController.Configuration)

Initializes and configures a Safari view controller that loads the specified URL.

convenience init(url: URL)

Initializes a Safari view controller that loads the specified URL.

init(url: URL, entersReaderIfAvailable: Bool)

Initializes a Safari view controller that will load the specified URL, entering Reader mode if Reader mode is requested and available.

Deprecated

