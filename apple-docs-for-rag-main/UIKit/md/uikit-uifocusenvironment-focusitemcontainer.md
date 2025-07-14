

- UIKit
- UIFocusEnvironment
-  focusItemContainer 

Instance Property

# focusItemContainer

The container for the child focus items in this focus environment.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+tvOS 12.0+visionOS 1.0+

``` source
@MainActor
var focusItemContainer: (any UIFocusItemContainer)? { get }
```

**Required**

## Discussion

The value of this property is `nil` when no container exists.

## See Also

### Checking the ancestry of the environment

func contains(any UIFocusEnvironment) -> Bool

Returns a Boolean value that indicates whether the focus environment contains the specified environment.

var parentFocusEnvironment: (any UIFocusEnvironment)?

The parent focus environment for this environment.

**Required**

