

- UIKit
- UIFocusEnvironment
-  contains(\_:) 

Instance Method

# contains(\_:)

Returns a Boolean value that indicates whether the focus environment contains the specified environment.

iOS 11.0+iPadOS 11.0+Mac CatalysttvOS 11.0+visionOS

``` source
@MainActor @preconcurrency
func contains(_ environment: any UIFocusEnvironment) -> Bool
```

## Parameters 

`environment`  

The focus environment to check.

## Return Value

true if `environment` is contained by the current focus environment or false if it is not.

## See Also

### Checking the ancestry of the environment

var parentFocusEnvironment: (any UIFocusEnvironment)?

The parent focus environment for this environment.

**Required**

var focusItemContainer: (any UIFocusItemContainer)?

The container for the child focus items in this focus environment.

**Required**

