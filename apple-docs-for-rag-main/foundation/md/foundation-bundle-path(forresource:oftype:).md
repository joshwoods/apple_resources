

- Foundation
- Bundle
-  path(forResource:ofType:) 

Instance Method

# path(forResource:ofType:)

Returns the full pathname for the resource identified by the specified name and file extension.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func path(
    forResource name: String?,
    ofType ext: String?
) -> String?
```

## Parameters 

`name`  

The name of the resource file.

If you specify `nil`, the method returns the first resource file it finds with the specified extension.

`ext`  

The filename extension of the file to locate.

If you specify an empty string or `nil`, the extension is assumed not to exist and the file is the first file encountered that exactly matches `name`.

## Return Value

The full pathname for the resource file, or `nil` if the file could not be located.

## Discussion

The method first looks for a matching resource file in the non-localized resource directory of the specified bundle. If a matching resource file is not found, it then looks in the top level of an available language-specific `.lproj` folder. (The search order for the language-specific folders corresponds to the user’s preferences.) It does not recurse through other subfolders at any of these locations. For more details on how localized resources are found, read The Bundle Search Pattern in Bundle Programming Guide.

The following code fragment gets the path to a plist within the bundle, and loads it into an `NSDictionary`:

```
NSBundle *thisBundle = [NSBundle bundleForClass:[self class]];
if (commonDictionaryPath = [thisBundle pathForResource:@"CommonDictionary" ofType:@"plist"]) {
    theDictionary = [[NSDictionary alloc] initWithContentsOfFile:commonDictionaryPath];
}
```

## See Also

### Finding Resource Files

func url(forResource: String?, withExtension: String?, subdirectory: String?) -> URL?

Returns the file URL for the resource file identified by the specified name and extension and residing in a given bundle directory.

func url(forResource: String?, withExtension: String?) -> URL?

Returns the file URL for the resource identified by the specified name and file extension.

func urls(forResourcesWithExtension: String?, subdirectory: String?) -> [URL]?

Returns an array of file URLs for all resources identified by the specified file extension and located in the specified bundle subdirectory.

func url(forResource: String?, withExtension: String?, subdirectory: String?, localization: String?) -> URL?

Returns the file URL for the resource identified by the specified name and file extension, located in the specified bundle subdirectory, and limited to global resources and those associated with the specified localization.

func urls(forResourcesWithExtension: String?, subdirectory: String?, localization: String?) -> [URL]?

Returns an array containing the file URLs for all bundle resources having the specified filename extension, residing in the specified resource subdirectory, and limited to global resources and those associated with the specified localization.

class func url(forResource: String?, withExtension: String?, subdirectory: String?, in: URL) -> URL?

Creates and returns a file URL for the resource with the specified name and extension in the specified bundle.

class func urls(forResourcesWithExtension: String?, subdirectory: String?, in: URL) -> [URL]?

Returns an array containing the file URLs for all bundle resources having the specified filename extension, residing in the specified resource subdirectory, within the specified bundle.

func path(forResource: String?, ofType: String?, inDirectory: String?) -> String?

Returns the full pathname for the resource identified by the specified name and file extension and located in the specified bundle subdirectory.

func path(forResource: String?, ofType: String?, inDirectory: String?, forLocalization: String?) -> String?

Returns the full pathname for the resource identified by the specified name and file extension, located in the specified bundle subdirectory, and limited to global resources and those associated with the specified localization.

func paths(forResourcesOfType: String?, inDirectory: String?) -> [String]

Returns an array containing the pathnames for all bundle resources having the specified filename extension and residing in the resource subdirectory.

func paths(forResourcesOfType: String?, inDirectory: String?, forLocalization: String?) -> [String]

Returns an array containing the file for all bundle resources having the specified filename extension, residing in the specified resource subdirectory, and limited to global resources and those associated with the specified localization.

class func path(forResource: String?, ofType: String?, inDirectory: String) -> String?

Returns the full pathname for the resource file identified by the specified name and extension and residing in a given bundle directory.

class func paths(forResourcesOfType: String?, inDirectory: String) -> [String]

Returns an array containing the pathnames for all bundle resources having the specified extension and residing in the bundle directory at the specified path.

