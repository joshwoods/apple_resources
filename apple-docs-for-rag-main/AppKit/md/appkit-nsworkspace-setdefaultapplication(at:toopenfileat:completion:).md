

- AppKit
- NSWorkspace
-  setDefaultApplication(at:toOpenFileAt:completion:) 

Instance Method

# setDefaultApplication(at:toOpenFileAt:completion:)

Sets the default app to use when opening a specific file.

macOS 12.0+

``` source
func setDefaultApplication(
    at applicationURL: URL,
    toOpenFileAt url: URL,
    completion completionHandler: (((any Error)?) -> Void)? = nil
)
```

``` source
func setDefaultApplication(
    at applicationURL: URL,
    toOpenFileAt url: URL
) async throws
```

## Parameters 

`applicationURL`  

The URL of the default app to use when opening the file.

`url`  

The URL of the file to open.

`completionHandler`  

The completion handler to call after the operation completes.

## Discussion

This method sets the default app to use for a specific file (rather than all files of that content type). The system requires write access to the specified `url` before it can make the change.

If a change requires user consent, the system asks the user for consent asynchronously before invoking the completion handler.

This function doesn’t apply to non-file URLs.

## See Also

### Setting Default Application Information

func setDefaultApplication(at: URL, toOpen: UTType, completion: (((any Error)?) -> Void)?)

Sets the default app to use when opening files of a specific content type.

func setDefaultApplication(at: URL, toOpenContentTypeOfFileAt: URL, completion: (((any Error)?) -> Void)?)

Sets the default app to use when opening files of a specific content type defined by a file URL.

func setDefaultApplication(at: URL, toOpenURLsWithScheme: String, completion: (((any Error)?) -> Void)?)

Sets the default app to use when opening files of a specific scheme.

