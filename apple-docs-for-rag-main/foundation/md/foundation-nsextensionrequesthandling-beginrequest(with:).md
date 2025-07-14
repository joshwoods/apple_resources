

- Foundation
- NSExtensionRequestHandling
-  beginRequest(with:) 

Instance Method

# beginRequest(with:)

Tells the extension to prepare for a host app’s request.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func beginRequest(with context: NSExtensionContext)
```

**Required**

## Parameters 

`context`  

An NSExtensionContext object that represents the context in which the host app makes the request. Typically, the context contains data that the extension can work on.

## Discussion

An extension prepares for a host app’s request by getting the context passed in this method and requesting related data items, if appropriate. This method is received after the extension is initialized, but before the principal object is asked to do anything with the context. For example, if the principal object is a view controller, it receives this message before loadView() is called. After an extension receives this message, the extensionContext property of the view controller returns a non`nil` value.

If your subclass conforms to this protocol and overrides `beginRequestWithExtensionContext:`, the subclass is expected to call `[super beginRequestWithExtensionContext:]`.

## See Also

### Related Documentation

App Extension Programming Guide

