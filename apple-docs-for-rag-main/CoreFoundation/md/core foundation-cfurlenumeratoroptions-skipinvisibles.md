

- Core Foundation
- CFURLEnumeratorOptions
-  skipInvisibles 

Type Property

# skipInvisibles

The enumerator skips “hidden” or “invisible” objects.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static var skipInvisibles: CFURLEnumeratorOptions { get }
```

## See Also

### Constants

static var descendRecursively: CFURLEnumeratorOptions

The enumerator recurses into each subdirectory enumerated.

static var generateFileReferenceURLs: CFURLEnumeratorOptions

The enumerator generates file reference URLs instead of file path URLs.

static var skipPackageContents: CFURLEnumeratorOptions

The enumerator skips package directory contents.

static var includeDirectoriesPreOrder: CFURLEnumeratorOptions

If provided along with the descendRecursively option, the recursive enumerator returns a directory’s URL before returning the URLs of the directory’s descendents.

static var includeDirectoriesPostOrder: CFURLEnumeratorOptions

If provided along with the descendRecursively option, the recursive enumerator returns a directory’s URL after returning the URLs of the directory’s descendents.

