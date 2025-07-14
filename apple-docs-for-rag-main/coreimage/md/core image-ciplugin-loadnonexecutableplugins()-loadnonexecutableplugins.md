

- Core Image
- CIPlugIn
-  loadNonExecutablePlugIns() 

Type Method

# loadNonExecutablePlugIns()

Scans directories for plugins.

macOS 10.4+

``` source
class func loadNonExecutablePlugIns()
```

## Discussion

This call scans for plugins with the extension `.plugin` in the following directories:

- /Library/Graphics/Image Units

- ~Library/Graphics/Image Units

This call adds new plug-ins. It doesn’t remove any plug-ins.

## See Also

### Loading Plug-ins

class func loadNonExecutablePlugIn(URL!)

Loads a non-executable plug-in specified by its URL.

