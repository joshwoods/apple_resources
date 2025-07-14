

- iTunes Library
- ITLibrary
-  init(apiVersion:options:) 

Initializer

# init(apiVersion:options:)

Initializes an instance of `ITLibrary` that can retrieve media entities.

Mac Catalyst 14.0+macOS 10.14+

``` source
init(
    apiVersion requestedAPIVersion: String,
    options: ITLibInitOptions
) throws
```

## Parameters 

`requestedAPIVersion`  

The version of the iTunesLibrary API that the app is requesting. Provide `"1.0"` if unknown.

`options`  

Options that change the initialization behavior. See ITLibInitOptions.

## Return Value

An ITLibrary instance that can retrieve media entities, or `nil` if the method fails.

## Discussion

Unless you specify the ITLibInitOptions.lazyLoadData option, the system reads and parses the default iTunes database for the current user during initialization of the ITLibrary class. All media entities cache in memory until deallocation of the object occurs.

## See Also

### Essentials

convenience init(apiVersion: String) throws

Initializes an instance of ITLibrary that can retrieve media entities.

enum ITLibInitOptions

These constants describe initialization options for an iTunes library.

