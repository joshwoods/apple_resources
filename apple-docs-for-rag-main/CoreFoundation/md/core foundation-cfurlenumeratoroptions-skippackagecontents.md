

- Core Foundation
- CFURLEnumeratorOptions
-  skipPackageContents 

Type Property

# skipPackageContents

The enumerator skips package directory contents.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static var skipPackageContents: CFURLEnumeratorOptions { get }
```

## Discussion

This option applies only to directory enumerators.

## See Also

### Constants

static var descendRecursively: CFURLEnumeratorOptions

The enumerator recurses into each subdirectory enumerated.

static var skipInvisibles: CFURLEnumeratorOptions

The enumerator skips “hidden” or “invisible” objects.

static var generateFileReferenceURLs: CFURLEnumeratorOptions

The enumerator generates file reference URLs instead of file path URLs.

static var includeDirectoriesPreOrder: CFURLEnumeratorOptions

If provided along with the descendRecursively option, the recursive enumerator returns a directory’s URL before returning the URLs of the directory’s descendents.

static var includeDirectoriesPostOrder: CFURLEnumeratorOptions

If provided along with the descendRecursively option, the recursive enumerator returns a directory’s URL after returning the URLs of the directory’s descendents.

