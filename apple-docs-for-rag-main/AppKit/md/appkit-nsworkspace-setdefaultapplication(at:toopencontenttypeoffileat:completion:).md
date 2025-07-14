

- AppKit
- NSWorkspace
-  setDefaultApplication(at:toOpenContentTypeOfFileAt:completion:) 

Instance Method

# setDefaultApplication(at:toOpenContentTypeOfFileAt:completion:)

Sets the default app to use when opening files of a specific content type defined by a file URL.

macOS 12.0+

``` source
func setDefaultApplication(
    at applicationURL: URL,
    toOpenContentTypeOfFileAt url: URL,
    completion completionHandler: (((any Error)?) -> Void)? = nil
)
```

``` source
func setDefaultApplication(
    at applicationURL: URL,
    toOpenContentTypeOfFileAt url: URL
) async throws
```

## Parameters 

`applicationURL`  

The URL of the default application.

`url`  

The URL of the file specifying the content type to open.

`completionHandler`  

The completion handler to call after the operation completes.

## Discussion

This method sets the default app to open files of the type specified by the file `url`. If a change requires user consent, the system asks the user for consent asynchronously before invoking the completion handler.

## See Also

### Setting Default Application Information

func setDefaultApplication(at: URL, toOpenFileAt: URL, completion: (((any Error)?) -> Void)?)

Sets the default app to use when opening a specific file.

func setDefaultApplication(at: URL, toOpen: UTType, completion: (((any Error)?) -> Void)?)

Sets the default app to use when opening files of a specific content type.

func setDefaultApplication(at: URL, toOpenURLsWithScheme: String, completion: (((any Error)?) -> Void)?)

Sets the default app to use when opening files of a specific scheme.

