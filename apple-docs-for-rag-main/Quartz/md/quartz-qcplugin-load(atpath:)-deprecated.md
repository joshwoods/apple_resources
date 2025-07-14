

- Quartz
- QCPlugIn
-  load(atPath:) Deprecated

Type Method

# load(atPath:)

Loads a Quartz Composer plug-in bundle from the specified path.

macOS 10.4–10.15Deprecated

``` source
class func load(atPath path: String!) -> Bool
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Parameters 

`path`  

The location of the bundle.

## Return Value

true if successful.

## Discussion

Call this method only if you need to load a plug-in bundle from a nonstandard location. Typically you don’t need to call this method because Quartz Composer automatically loads bundles that you install in one of the following locations:

- `/Library/Graphics/Quartz Composer Plug-Ins`

- `~/Library/Graphics/Quartz Composer Plug-Ins`

This method does nothing if the bundle is already loaded. (This method does not load in all environments. Web Kit, for example, cannot load custom patches.)

The bundle can contain more than one `QCPlugIn` subclass. After the bundle is loaded, each `QCPlugIn` subclass appears as a patch in the Quartz Composer patch library.

## See Also

### Loading Bundle and Custom Patches Manually

class func registerClass(AnyClass!)

Registers a `QCPlugIn` subclass.

Deprecated

