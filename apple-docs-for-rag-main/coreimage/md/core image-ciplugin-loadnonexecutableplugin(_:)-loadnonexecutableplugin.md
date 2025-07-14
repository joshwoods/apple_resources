

- Core Image
- CIPlugIn
-  loadNonExecutablePlugIn(\_:) 

Type Method

# loadNonExecutablePlugIn(\_:)

Loads a non-executable plug-in specified by its URL.

macOS 10.15+

``` source
class func loadNonExecutablePlugIn(_ url: URL!)
```

## Parameters 

`url`  

The location of the plugin to load.

## Discussion

If the filters contain executable code the plugin isn’t loaded.

## See Also

### Loading Plug-ins

class func loadNonExecutablePlugIns()

Scans directories for plugins.

