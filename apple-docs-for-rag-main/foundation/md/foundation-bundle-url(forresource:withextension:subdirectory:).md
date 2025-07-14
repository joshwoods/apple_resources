

- Foundation
- Bundle
-  url(forResource:withExtension:subdirectory:) 

Instance Method

# url(forResource:withExtension:subdirectory:)

Returns the file URL for the resource file identified by the specified name and extension and residing in a given bundle directory.

iOS 4.0+iPadOS 4.0+Mac Catalyst 13.1+macOS 10.6+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func url(
    forResource name: String?,
    withExtension ext: String?,
    subdirectory subpath: String?
) -> URL?
```

## Parameters 

`name`  

The name of a resource file contained in the directory specified by `subpath`.

If you specify `nil`, the method returns the first resource file it finds with the specified extension in that directory.

`ext`  

The filename extension of the file to locate.

If you specify an empty string or `nil`, the extension is assumed not to exist and the file URL is the first file encountered that exactly matches `name`.

`subpath`  

The path of a top-level bundle directory. This must be a valid path. For example, to specify the bundle directory for a Mac app, you might specify the path `/Applications/MyApp.app`.

## Return Value

The file URL for the resource file or `nil` if the file could not be located. This method also returns `nil` if the bundle specified by the `bundlePath` parameter does not exist or is not a readable directory.

## Discussion

For details on how localized resources are found, read The Bundle Search Pattern in Bundle Programming Guide.

## See Also

### Finding Resource Files

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

func path(forResource: String?, ofType: String?) -> String?

Returns the full pathname for the resource identified by the specified name and file extension.

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

