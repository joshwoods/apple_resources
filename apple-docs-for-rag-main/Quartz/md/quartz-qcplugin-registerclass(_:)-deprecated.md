

- Quartz
- QCPlugIn
-  registerClass(\_:) Deprecated

Type Method

# registerClass(\_:)

Registers a `QCPlugIn` subclass.

macOS 10.4–10.15Deprecated

``` source
class func registerClass(_ aClass: AnyClass!)
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Parameters 

`aClass`  

The `QCPlugIn` subclass.

## Discussion

You call this method only if the code for your custom patch is mixed with your application code, and you plan only to use the custom patch from within your application.

## See Also

### Loading Bundle and Custom Patches Manually

class func load(atPath: String!) -> Bool

Loads a Quartz Composer plug-in bundle from the specified path.

Deprecated

