

- Social
- SLComposeServiceViewController
-  cancel() 

Instance Method

# cancel()

Starts the animated dismissal of the compose view.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+

``` source
@MainActor
func cancel()
```

## Discussion

When the cancel animation finishes, this method calls didSelectCancel(). A subclass shouldn’t need to override `cancel`. In rare cases a subclass may call `cancel`, such as in response to a catastrophic failure during user interaction with the compose view.

