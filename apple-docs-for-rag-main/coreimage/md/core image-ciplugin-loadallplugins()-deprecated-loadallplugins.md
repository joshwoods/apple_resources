

- Core Image
- CIPlugIn
-  loadAllPlugIns() Deprecated

Type Method

# loadAllPlugIns()

Scans directories for files that have the `.plugin` extension and then loads the image units.

macOS 10.4–10.15Deprecated

``` source
class func loadAllPlugIns()
```

## Discussion

This method scans the following directories:

- `/Library/Graphics/Image Units`

- ~`/Library/Graphics/Image Units`

Call this method once. If you call this method more than once, Core Image loads newly added image units, but image units (and the filters they contain) that are already loaded are not removed.

## See Also

### Deprecated

class func load(URL!, allowExecutableCode: Bool)

Loads filters from an image unit that have the appropriate executable status.

Deprecated

### Related Documentation

Image Unit Tutorial

Core Image Programming Guide

