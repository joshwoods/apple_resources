

- UIKit
- UIScene
-  UIScene.OpenURLOptions 

Class

# UIScene.OpenURLOptions

Options that UIKit provides when asking your app to open a URL.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
class OpenURLOptions
```

## Overview

Don’t create a UIScene.OpenURLOptions object directly. UIKit creates one for you when your app receives a request to open a URL. Use the information in the object to determine how to respond to the URL.

## Topics

### Specifying the URL details

var sourceApplication: String?

The bundle ID of the app that originated the request.

var annotation: Any?

A property-list object that contains the annotation data provided by a document interaction controller.

var eventAttribution: UIEventAttribution?

An event attribution associated with the URL to open.

### Specifying the behavior options

var openInPlace: Bool

A Boolean value that indicates whether you should open the URL at its current location instead of copying it to your app’s container.

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

## See Also

### Getting the URL

var url: URL

The URL to open.

var options: UIScene.OpenURLOptions

Additional information for determining how to open the URL.

