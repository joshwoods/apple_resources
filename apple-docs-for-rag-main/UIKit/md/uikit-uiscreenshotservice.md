

- UIKit
-  UIScreenshotService 

Class

# UIScreenshotService

An object that coordinates the creation of PDF screenshots of an app’s content.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+

``` source
@MainActor
class UIScreenshotService
```

## Overview

When people take a screenshot of your app’s content, you work with a UIScreenshotService object to provide a PDF version of that screenshot. You don’t create a UIScreenshotService object directly. Instead, you retrieve the object from the screenshotService property of your window scene and assign a delegate to it. Then when people take a screenshot, UIKit asks your delegate for the PDF data.

For information about how to provide the PDF data, see UIScreenshotServiceDelegate.

Tip

Beginning in iOS 17 and iPadOS 17, people have the option to share or save the generated full page screenshot as a PDF or an image.

## Topics

### Responding to screenshot requests

var delegate: (any UIScreenshotServiceDelegate)?

The custom object you use to provide PDF data for a screenshot.

protocol UIScreenshotServiceDelegate

Methods you use to generate PDF data that accompanies a user-requested screenshot.

### Getting the current scene

var windowScene: UIWindowScene?

The window scene that contains the windows to capture in your PDF data.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

