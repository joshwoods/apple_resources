

- WebKit
-  WebPlugInViewFactory Deprecated

Protocol

# WebPlugInViewFactory

macOS 10.3–10.14Deprecated

``` source
protocol WebPlugInViewFactory : NSObjectProtocol
```

## Topics

### Type Methods

static func plugInView(withArguments: [AnyHashable : Any]!) -> NSView!

Creates a new plug-in view.

**Required**

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Related Documentation

WebKit Objective-C Programming Guide

### Implementing Plugins (Legacy)

WebPlugIn

The \`WebPlugIn\` informal protocol defines methods that enable interaction between an application using the WebKit framework and any WebKit-based plug-ins it may use.

WebPlugInContainer

\`WebPlugInContainer\` is an informal protocol that enables a plug-in to send messages to the application.

