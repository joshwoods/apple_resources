

- Social
- SLComposeServiceViewController
-  didSelectPost() 

Instance Method

# didSelectPost()

Sent to the compose view after the post animation finishes.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+

``` source
@MainActor
func didSelectPost()
```

## Discussion

By default, this method calls the completeRequestReturningItems: method of the associated extensionContext property, passing `nil` in the `items` array and a `nil` expiration handler. You must override `didSelectPost` to perform the post of contentText and any attachments. In your implementation of this method, you can call `super` to take advantage of the default completion handler; if you don’t call `super`, you must call the completion method of the extension context.

## See Also

### Responding to Lifecycle Events

func presentationAnimationDidFinish()

Tells the compose view controller that the presentation animation is finished.

func didSelectCancel()

Sent to the compose view after the cancel animation finishes.

