

- Social
- SLComposeServiceViewController
-  validateContent() 

Instance Method

# validateContent()

Performs validation of the current content and updates the state of the Post button, if appropriate.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+

``` source
@MainActor
func validateContent()
```

## Discussion

By default, `validateContent` calls isContentValid(), performs internal content validation, and updates the state of the Post button, if necessary. You should call this method if you change any data that your implementation of `isContentValid` uses to test for content validity.

## See Also

### Validating Content

var charactersRemaining: NSNumber!

The number of characters remaining in a custom character limit.

func isContentValid() -> Bool

A Boolean value that indicates whether the current content and attachments are valid.

