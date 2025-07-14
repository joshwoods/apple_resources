

- Social
- SLComposeServiceViewController
-  presentationAnimationDidFinish() 

Instance Method

# presentationAnimationDidFinish()

Tells the compose view controller that the presentation animation is finished.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+

``` source
@MainActor
func presentationAnimationDidFinish()
```

## Discussion

Implement this method to avoid performing lengthy work during initialization or the iOS view controller methods viewWillAppear(_:) and viewDidAppear(_:).

## See Also

### Responding to Lifecycle Events

func didSelectCancel()

Sent to the compose view after the cancel animation finishes.

func didSelectPost()

Sent to the compose view after the post animation finishes.

