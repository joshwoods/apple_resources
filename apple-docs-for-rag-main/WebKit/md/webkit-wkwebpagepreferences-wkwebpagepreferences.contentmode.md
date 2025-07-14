

- WebKit
- WKWebpagePreferences
-  WKWebpagePreferences.ContentMode 

Enumeration

# WKWebpagePreferences.ContentMode

Constants that indicate how to render web view content.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOSvisionOS 1.0+

``` source
enum ContentMode
```

## Overview

Browsers often render webpages differently based on device type. For example, Safari provides a desktop-class experience when displaying webpages on Mac and iPad, but it displays a mobile experience when displaying pages on iPhone. Use content modes to specify how you want your web view to render content within your app.

## Topics

### Getting the Content Modes

case recommended

The content mode that is appropriate for the current device.

case desktop

The content mode that represents a desktop experience.

case mobile

The content mode that represents a mobile experience.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Setting the preferred content mode

var preferredContentMode: WKWebpagePreferences.ContentMode

The content mode for the web view to use when it loads and renders a webpage.

