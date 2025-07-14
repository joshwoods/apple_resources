

- iTunes Library
- ITLibrary
-  init(apiVersion:) 

Initializer

# init(apiVersion:)

Initializes an instance of ITLibrary that can retrieve media entities.

Mac Catalyst 14.0+macOS 10.13+

``` source
convenience init(apiVersion requestedAPIVersion: String) throws
```

## Parameters 

`requestedAPIVersion`  

The version of the iTunesLibrary API that the app is requesting. Provide `"1.0"` if unknown.

## Return Value

An ITLibrary instance that can retrieve media entities, or `nil` if the method fails.

## Discussion

During initialization of the ITLibrary class, the system reads and parses the default iTunes database for the current user. All media entities cache in memory until deallocation of the object occurs.

Listing 1.

```
#import 

NSError * error = nil;
ITLibrary* library = [[ITLibrary alloc] initWithAPIVersion:@"1.0" error:&error];
if (library)
{
  NSArray playlists = library.allPlaylists; //  

## See Also

### Essentials

init(apiVersion: String, options: ITLibInitOptions) throws

Initializes an instance of `ITLibrary` that can retrieve media entities.

enum ITLibInitOptions

These constants describe initialization options for an iTunes library.

