

- Safari Services
-  SFAddToHomeScreenInfo 

Class

# SFAddToHomeScreenInfo

A class that provides information about a web app that someone adds to their Home Screen.

iOS 18.2+iPadOS 18.2+visionOS 2.2+

``` source
class SFAddToHomeScreenInfo
```

## Overview

Create an instance of `SFAddToHomeScreenInfo` in your getHomeScreenWebAppInfo(completionHandler:) implementation. Configure the object with the web app’s manifest and the cookies your browser uses with the web app, then pass the object to the method’s completion handler.

## Topics

### Creating an information object

init(manifest: BEWebAppManifest)

Initializes a Home Screen information object with the supplied web app manifest.

### Information about a web app

var manifest: BEWebAppManifest

var websiteCookies: [HTTPCookie]

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

### Providing information about a web app to the system

func getHomeScreenWebAppInfo(completionHandler: (SFAddToHomeScreenInfo?) -> Void)

Provides information about a web app to the system.

func getWebAppManifest(completionHandler: (BEWebAppManifest?) -> Void)

Provides the web app’s manifest to the system, if the bookmark represents a web app.

