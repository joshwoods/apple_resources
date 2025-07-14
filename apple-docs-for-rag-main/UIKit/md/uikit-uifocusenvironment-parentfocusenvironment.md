

- UIKit
- UIFocusEnvironment
-  parentFocusEnvironment 

Instance Property

# parentFocusEnvironment

The parent focus environment for this environment.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+tvOS 12.0+visionOS 1.0+

``` source
@MainActor
weak var parentFocusEnvironment: (any UIFocusEnvironment)? { get }
```

**Required**

## Discussion

The value of this property is `nil` when no parent container exists.

## See Also

### Checking the ancestry of the environment

func contains(any UIFocusEnvironment) -> Bool

Returns a Boolean value that indicates whether the focus environment contains the specified environment.

var focusItemContainer: (any UIFocusItemContainer)?

The container for the child focus items in this focus environment.

**Required**

