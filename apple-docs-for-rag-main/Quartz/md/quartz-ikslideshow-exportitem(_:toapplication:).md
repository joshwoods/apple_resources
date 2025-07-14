

- Quartz
- IKSlideshow
-  exportItem(\_:toApplication:) 

Type Method

# exportItem(\_:toApplication:)

Exports a slideshow item to the application that has the provided bundle identifier.

macOS 10.4+

``` source
class func exportItem(
    _ item: Any!,
    toApplication applicationBundleIdentifier: String!
)
```

## Parameters 

`item`  

The item to export

`applicationBundleIdentifier`  

The bundle identifier of the application that you want to export the item to.

## See Also

### Exporting Slideshow Items

class func canExport(toApplication: String!) -> Bool

Finds out whether the slideshow can export its contents to an application.

