

- AppKit
- NSWorkspace
-  setDefaultApplication(at:toOpen:completion:) 

Instance Method

# setDefaultApplication(at:toOpen:completion:)

Sets the default app to use when opening files of a specific content type.

macOS 12.0+

``` source
func setDefaultApplication(
    at applicationURL: URL,
    toOpen contentType: UTType,
    completion completionHandler: (((any Error)?) -> Void)? = nil
)
```

``` source
func setDefaultApplication(
    at applicationURL: URL,
    toOpen contentType: UTType
) async throws
```

## Parameters 

`applicationURL`  

The URL of the default application.

`contentType`  

The content type to open.

`completionHandler`  

The completion handler to call after the operation completes.

## Discussion

This method sets the default app to open for files of the specified `contentType`. If a change requires user consent, the system asks the user for consent asynchronously before invoking the completion handler.

## See Also

### Setting Default Application Information

func setDefaultApplication(at: URL, toOpenFileAt: URL, completion: (((any Error)?) -> Void)?)

Sets the default app to use when opening a specific file.

func setDefaultApplication(at: URL, toOpenContentTypeOfFileAt: URL, completion: (((any Error)?) -> Void)?)

Sets the default app to use when opening files of a specific content type defined by a file URL.

func setDefaultApplication(at: URL, toOpenURLsWithScheme: String, completion: (((any Error)?) -> Void)?)

Sets the default app to use when opening files of a specific scheme.

