

- Social
- SLComposeViewController
-  completionHandler 

Instance Property

# completionHandler

The handler to call when the user is done composing a post.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+

``` source
@MainActor
var completionHandler: SLComposeViewControllerCompletionHandler! { get set }
```

## Discussion

The handler has a single parameter that indicates whether the user finished or cancelled composing the post. This block is not guaranteed to be called on any particular thread. Do not dismiss the SLComposeViewController in your completion handler—the system will do so automatically.

## See Also

### Processing the Results

typealias SLComposeViewControllerCompletionHandler

Defines a handler to call when the user finishes composing a post.

enum SLComposeViewControllerResult

Possible values for the `result` parameter of the completionHandler property.

