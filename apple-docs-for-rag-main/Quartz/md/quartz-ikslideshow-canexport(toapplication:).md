

- Quartz
- IKSlideshow
-  canExport(toApplication:) 

Type Method

# canExport(toApplication:)

Finds out whether the slideshow can export its contents to an application.

macOS 10.4+

``` source
class func canExport(toApplication applicationBundleIdentifier: String!) -> Bool
```

## Parameters 

`applicationBundleIdentifier`  

The bundle identifier of the application that you want to export the slideshow to. See Bundle Identifiers.

## Return Value

true if the slideshow can be exported to the specified application; false otherwise.

## See Also

### Exporting Slideshow Items

class func exportItem(Any!, toApplication: String!)

Exports a slideshow item to the application that has the provided bundle identifier.

