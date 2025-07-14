

- Core Foundation
- CFURLEnumeratorOptions
-  descendRecursively 

Type Property

# descendRecursively

The enumerator recurses into each subdirectory enumerated.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static var descendRecursively: CFURLEnumeratorOptions { get }
```

## Discussion

This option applies only to directory enumerators.

You can enumerate the directories that a recursive enumerator encounters in pre-order fashion, post-order fashion, or both, by providing a combination of the includeDirectoriesPreOrder and includeDirectoriesPostOrder options. If you provide neither option, the recursive enumerator behaves as if it was provided the includeDirectoriesPreOrder option.

## See Also

### Constants

static var skipInvisibles: CFURLEnumeratorOptions

The enumerator skips “hidden” or “invisible” objects.

static var generateFileReferenceURLs: CFURLEnumeratorOptions

The enumerator generates file reference URLs instead of file path URLs.

static var skipPackageContents: CFURLEnumeratorOptions

The enumerator skips package directory contents.

static var includeDirectoriesPreOrder: CFURLEnumeratorOptions

If provided along with the descendRecursively option, the recursive enumerator returns a directory’s URL before returning the URLs of the directory’s descendents.

static var includeDirectoriesPostOrder: CFURLEnumeratorOptions

If provided along with the descendRecursively option, the recursive enumerator returns a directory’s URL after returning the URLs of the directory’s descendents.

