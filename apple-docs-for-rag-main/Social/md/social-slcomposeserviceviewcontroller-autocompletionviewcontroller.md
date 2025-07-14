

- Social
- SLComposeServiceViewController
-  autoCompletionViewController 

Instance Property

# autoCompletionViewController

The view controller that manages an autocompletion view for suggesting common text completions while users type.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+

``` source
@MainActor
var autoCompletionViewController: UIViewController! { get set }
```

## Discussion

An autocompletion view can appear in place of the list of configuration items, just below the text view in the compose view. The compose view controller allows only one autocompletion view controller to be present at a time.

Note that your custom autocompletion view controller should set its preferredContentSize property to an appropriate value. `SLComposeServiceViewController` observes changes to the preferredContentSize property and animates view size changes, if necessary.

