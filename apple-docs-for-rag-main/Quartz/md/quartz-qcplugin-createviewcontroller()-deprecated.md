

- Quartz
- QCPlugIn
-  createViewController() Deprecated

Instance Method

# createViewController()

Creates and returns a view controller for the Settings pane of a custom patch.

macOS 10.4–10.15Deprecated

``` source
func createViewController() -> QCPlugInViewController!
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Return Value

A view controller for the custom patch. Quartz Composer releases the controller when it is no longer needed. If necessary, you can return a subclass of `QCPlugInViewController`, but this it not typically done.

## Discussion

This extension to the `QCPlugInViewController` class provides user-interface support for the Settings pane of the inspector for a custom patch. You must override this method if your custom patch provides a Settings pane. The `QCPlugInViewController` object acts as a controller for Cocoa bindings between the custom patch instance (the model) and the `NSView` that contains the controls. It loads the nib file from the bundle.

The implementation is straightforward. You allocate a `QCPlugInViewController` object, initialize it, and provide the name of the nib file that contains the user interface for the Settings pane.

Note that this method follows the Core Foundation “create” rule. See the ownership policy in Memory Management Programming Guide for Core Foundation.

For example, if the nib file name that contains the settings pane is `MySettingsPane.nib`, the implementation is:

```
```

## See Also

### Defining Internal Settings

class func plugInKeys() -> [Any]!

Returns the keys for the internal settings of a custom patch.

Deprecated

