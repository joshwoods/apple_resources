

- AppKit
- NSWorkspace
-  setDefaultApplication(at:toOpenURLsWithScheme:completion:) 

Instance Method

# setDefaultApplication(at:toOpenURLsWithScheme:completion:)

Sets the default app to use when opening files of a specific scheme.

macOS 12.0+

``` source
func setDefaultApplication(
    at applicationURL: URL,
    toOpenURLsWithScheme urlScheme: String,
    completion completionHandler: (((any Error)?) -> Void)? = nil
)
```

``` source
func setDefaultApplication(
    at applicationURL: URL,
    toOpenURLsWithScheme urlScheme: String
) async throws
```

## Parameters 

`applicationURL`  

The URL of the default application.

`urlScheme`  

The URL of the scheme to open.

`completionHandler`  

The completion handler to call after the operation completes.

## Discussion

This method sets the default app to open files of the type specified by the `urlScheme`. If a change requires user consent, the system asks the for consent asynchronously before invoking the completion handler.

## See Also

### Setting Default Application Information

func setDefaultApplication(at: URL, toOpenFileAt: URL, completion: (((any Error)?) -> Void)?)

Sets the default app to use when opening a specific file.

func setDefaultApplication(at: URL, toOpen: UTType, completion: (((any Error)?) -> Void)?)

Sets the default app to use when opening files of a specific content type.

func setDefaultApplication(at: URL, toOpenContentTypeOfFileAt: URL, completion: (((any Error)?) -> Void)?)

Sets the default app to use when opening files of a specific content type defined by a file URL.

