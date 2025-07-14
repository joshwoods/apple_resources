

- Social
-  SLComposeViewControllerCompletionHandler 

Type Alias

# SLComposeViewControllerCompletionHandler

Defines a handler to call when the user finishes composing a post.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.0+

``` source
typealias SLComposeViewControllerCompletionHandler = (SLComposeViewControllerResult) -> Void
```

## Discussion

The completion handler is called while the SLComposeViewController is still visible and it is responsible for dismissing the view controller. For the possible values of the `result` parameter, see SLComposeViewControllerResult. Use the completionHandler property to set this handler.

## See Also

### Processing the Results

var completionHandler: SLComposeViewControllerCompletionHandler!

The handler to call when the user is done composing a post.

enum SLComposeViewControllerResult

Possible values for the `result` parameter of the completionHandler property.

