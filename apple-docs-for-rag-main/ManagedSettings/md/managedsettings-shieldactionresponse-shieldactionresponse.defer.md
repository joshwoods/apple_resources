

- ManagedSettings
- ShieldActionResponse
-  ShieldActionResponse.defer 

Case

# ShieldActionResponse.defer

An instruction to defer a response to the action.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+

``` source
case `defer`
```

## Discussion

Use `defer` to delay an immediate response to a shield action; for example, if your extension on a client device sends a remote request to a parent or guardian’s device. When you specify this option, the shield redraws its UI, which gives your extension on the client device an opportunity to reconfigure the shield’s appearance.

## See Also

### Responses

case close

An instruction for the system to close the current application or web browser.

case none

An instruction that the system doesn’t need to take any additional action on behalf of the extension.

