

- WebKit
- WebPlugInViewFactory
-  plugInView(withArguments:) Deprecated

Type Method

# plugInView(withArguments:)

Creates a new plug-in view.

macOS 10.3–10.14Deprecated

``` source
static func plugInView(withArguments arguments: [AnyHashable : Any]!) -> NSView!
```

**Required**

## Parameters 

`arguments`  

Arguments used in creating the view.

## Return Value

The created view.

## Discussion

This method returns an `NSView` object that conforms to the `WebPlugIn` informal protocol. The arguments dictionary should be specified by the keys and objects described in `Constants`. This method is required.

