

- Social
- SLComposeServiceViewController
-  charactersRemaining 

Instance Property

# charactersRemaining

The number of characters remaining in a custom character limit.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+

``` source
@MainActor
var charactersRemaining: NSNumber! { get set }
```

## Discussion

Set this property to a non-`nil` value when you want to make the character count view appear in the compose view (changing the value redraws the character count view). The default value of this property is `nil`.

## See Also

### Validating Content

func isContentValid() -> Bool

A Boolean value that indicates whether the current content and attachments are valid.

func validateContent()

Performs validation of the current content and updates the state of the Post button, if appropriate.

