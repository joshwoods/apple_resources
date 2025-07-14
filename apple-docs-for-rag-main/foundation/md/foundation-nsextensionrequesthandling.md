

- Foundation
-  NSExtensionRequestHandling 

Protocol

# NSExtensionRequestHandling

The interface an app extension uses to respond to a request from a host app.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
protocol NSExtensionRequestHandling : NSObjectProtocol
```

## Overview

The NSExtensionRequestHandling protocol provides a life cycle hook into an app extension. An extension’s principal object can implement this protocol and use beginRequest(with:) to keep track of the request from a host app.

## Topics

### Preparing for a request

func beginRequest(with: NSExtensionContext)

Tells the extension to prepare for a host app’s request.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Extension Support

class NSExtensionContext

The host app context from which an app extension is invoked.

