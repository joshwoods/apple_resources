

- UIKit
-  UIOpenURLContext 

Class

# UIOpenURLContext

A system-provided object that contains the information you need to open a single URL.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
class UIOpenURLContext
```

## Overview

UIKit provides a UIOpenURLContext object when your app receives a URL to open. The object contains the URL itself and any options needed to handle the URL correctly. Don’t create UIOpenURLContext objects yourself.

## Topics

### Getting the URL

var url: URL

The URL to open.

var options: UIScene.OpenURLOptions

Additional information for determining how to open the URL.

class OpenURLOptions

Options that UIKit provides when asking your app to open a URL.

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

### URL management

class OpenExternalURLOptions

Options you specify when asking a scene to open a URL.

