

- WidgetKit
- ControlPushHandler
-  pushTokensDidChange(controls:) 

Instance Method

# pushTokensDidChange(controls:)

Handle push tokens changing for configured controls.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
func pushTokensDidChange(controls: [ControlInfo])
```

**Required**

## Parameters 

`controls`  

Information about controls that support push updates.

## Discussion

This function always provides information for all controls that support push updates even if only some of the tokens have changed.

