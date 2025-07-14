

- Social
- SLComposeServiceViewController
-  didSelectCancel() 

Instance Method

# didSelectCancel()

Sent to the compose view after the cancel animation finishes.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+

``` source
@MainActor
func didSelectCancel()
```

## Discussion

By default, this method calls the completeRequestReturningItems: method of the associated extensionContext property, passing the appropriate error value in the `items` array and a `nil` expiration.

## See Also

### Responding to Lifecycle Events

func presentationAnimationDidFinish()

Tells the compose view controller that the presentation animation is finished.

func didSelectPost()

Sent to the compose view after the post animation finishes.

