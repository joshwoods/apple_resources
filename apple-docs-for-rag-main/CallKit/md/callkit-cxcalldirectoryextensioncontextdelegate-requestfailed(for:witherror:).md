

- CallKit
- CXCallDirectoryExtensionContextDelegate
-  requestFailed(for:withError:) 

Instance Method

# requestFailed(for:withError:)

Called when a Call Directory app extension request fails.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+

``` source
func requestFailed(
    for extensionContext: CXCallDirectoryExtensionContext,
    withError error: any Error
)
```

**Required**

## Parameters 

`extensionContext`  

The extension context associated with the failed request.

`error`  

An error object containing information about the request failure.

