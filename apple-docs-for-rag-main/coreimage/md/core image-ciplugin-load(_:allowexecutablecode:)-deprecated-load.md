

- Core Image
- CIPlugIn
-  load(\_:allowExecutableCode:) Deprecated

Type Method

# load(\_:allowExecutableCode:)

Loads filters from an image unit that have the appropriate executable status.

macOS 10.7–10.15Deprecated

``` source
class func load(
    _ url: URL!,
    allowExecutableCode: Bool
)
```

## Parameters 

`url`  

The location of the image unit to load.

`allowExecutableCode`  

`true` to load all filters from the image unit, or `false` to load only those filters without CPU executable code.

## Discussion

You need to call this method only once to load a specific image unit. The behavior of this method is not defined for multiple calls for the same image unit. If you pass `false` for the `allowExecutableCode` parameter, Core Image will load only pure kernel filters that run entirely on the GPU, ignoring filters implemented using compiled Objective-C code.

## See Also

### Deprecated

class func loadAllPlugIns()

Scans directories for files that have the `.plugin` extension and then loads the image units.

Deprecated

