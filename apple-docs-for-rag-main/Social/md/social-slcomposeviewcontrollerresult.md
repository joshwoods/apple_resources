

- Social
-  SLComposeViewControllerResult 

Enumeration

# SLComposeViewControllerResult

Possible values for the `result` parameter of the completionHandler property.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.0+

``` source
enum SLComposeViewControllerResult
```

## Topics

### Constants

case cancelled

The view controller is dismissed without sending the post.

case done

The view controller is dismissed and the message is being sent in the background.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Processing the Results

var completionHandler: SLComposeViewControllerCompletionHandler!

The handler to call when the user is done composing a post.

typealias SLComposeViewControllerCompletionHandler

Defines a handler to call when the user finishes composing a post.

