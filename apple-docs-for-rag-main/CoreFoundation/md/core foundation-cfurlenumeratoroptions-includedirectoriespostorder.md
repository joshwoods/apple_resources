

- Core Foundation
- CFURLEnumeratorOptions
-  includeDirectoriesPostOrder 

Type Property

# includeDirectoriesPostOrder

If provided along with the descendRecursively option, the recursive enumerator returns a directory’s URL after returning the URLs of the directory’s descendents.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static var includeDirectoriesPostOrder: CFURLEnumeratorOptions { get }
```

## Discussion

A recursive post-order enumerator returns CFURLEnumeratorResult.directoryPostOrderSuccess when it returns a directory’s URL after returning the directory’s descendents.

## See Also

### Constants

static var descendRecursively: CFURLEnumeratorOptions

The enumerator recurses into each subdirectory enumerated.

static var skipInvisibles: CFURLEnumeratorOptions

The enumerator skips “hidden” or “invisible” objects.

static var generateFileReferenceURLs: CFURLEnumeratorOptions

The enumerator generates file reference URLs instead of file path URLs.

static var skipPackageContents: CFURLEnumeratorOptions

The enumerator skips package directory contents.

static var includeDirectoriesPreOrder: CFURLEnumeratorOptions

If provided along with the descendRecursively option, the recursive enumerator returns a directory’s URL before returning the URLs of the directory’s descendents.

