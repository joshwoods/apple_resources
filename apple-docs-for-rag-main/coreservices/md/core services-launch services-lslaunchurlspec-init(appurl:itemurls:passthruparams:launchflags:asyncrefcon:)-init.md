

- Core Services
- Launch Services
- LSLaunchURLSpec
-  init(appURL:itemURLs:passThruParams:launchFlags:asyncRefCon:) 

Initializer

# init(appURL:itemURLs:passThruParams:launchFlags:asyncRefCon:)

Create a launch URL with the provided parameters.

macOS 10.0+Xcode 9.0+

``` source
init(
    appURL: Unmanaged?,
    itemURLs: Unmanaged?,
    passThruParams: UnsafePointer?,
    launchFlags: LSLaunchFlags,
    asyncRefCon: UnsafeMutableRawPointer?
)
```

## Parameters 

`appURL`  

The URL of the application to launch.

`itemURLs`  

An array of URLs for the items to open.

`passThruParams`  

Optional parameters passed to the application without parsing.

`launchFlags`  

Flags specifying the launch behavior.

`asyncRefCon`  

A pointer to an arbitrary application-defined value notifying you of an application’s launch or termination.

## See Also

### Creating a Launch URL

init()

Create a launch URL.

### Related Documentation

struct LSLaunchURLSpec

The specification for launching an app, opening items, or both, along with related information.

