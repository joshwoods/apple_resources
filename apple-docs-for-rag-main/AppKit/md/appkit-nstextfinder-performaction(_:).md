

- AppKit
- NSTextFinder
-  performAction(\_:) 

Instance Method

# performAction(\_:)

Performs the specified text finding action.

macOS 10.7+

``` source
func performAction(_ op: NSTextFinder.Action)
```

## Parameters 

`op`  

The text finding action. See NSTextFinder.Action for the possible values.

## Discussion

Objects that respond to performTextFinderAction(_:) typically call validateAction(_:) to ensure that the action is valid and then invoke performAction(_:) if validation is successful.

When invoking the validateAction(_:) and performAction(_:) the item or sender’s tag should be passed as the parameter. By convention, the `sender` parameter for this method will have an NSTextFinder.Action set as its tag. The responder that receives this method should pass the tag as the action for this method:

```
- (void)performTextFinderAction:(id)sender {
    [self.textFinder performAction:[sender tag]];
}
```

## See Also

### Validating and Performing Text Finding

func validateAction(NSTextFinder.Action) -> Bool

Allows validation of the find action before performing.

func cancelFindIndicator()

Cancels the find indicator immediately.

