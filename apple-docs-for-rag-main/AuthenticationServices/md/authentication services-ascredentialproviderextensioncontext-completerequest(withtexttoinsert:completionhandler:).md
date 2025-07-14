

- Authentication Services
- ASCredentialProviderExtensionContext
-  completeRequest(withTextToInsert:completionHandler:) 

Instance Method

# completeRequest(withTextToInsert:completionHandler:)

Provides the user-selected text.

iOS 18.0+iPadOS 18.0+

``` source
func completeRequest(
    withTextToInsert text: String,
    completionHandler: ((Bool) -> Void)? = nil
)
```

``` source
func completeRequest(withTextToInsert text: String) async -> Bool
```

## Parameters 

`text`  

The text to insert.

`completionHandler`  

Optional work that the extension performs as a background-priority task after the request completes. The `expired` parameter is `YES` if the system prematurely terminates a previous non-expiration invocation of the `completionHandler`.

## Overview

At some point after you call this method, the system dismisses the associated view controller.

