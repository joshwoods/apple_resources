

- Social
- SLComposeServiceViewController
-  isContentValid() 

Instance Method

# isContentValid()

A Boolean value that indicates whether the current content and attachments are valid.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+

``` source
@MainActor
func isContentValid() -> Bool
```

## Return Value

true if the current content and attachments are valid for posting, otherwise false. The default return value is true.

## Discussion

This method is automatically called after each change a user makes to the text in the compose view. You can use this method to determine whether the Post button should be enabled and to update charactersRemaining, if necessary.

A subclass should implement this method to perform custom validation of the user’s content before initiating a post.

## See Also

### Validating Content

var charactersRemaining: NSNumber!

The number of characters remaining in a custom character limit.

func validateContent()

Performs validation of the current content and updates the state of the Post button, if appropriate.

