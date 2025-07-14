

- WatchKit
- WKExtension
-  openSystemURL(\_:) 

Instance Method

# openSystemURL(\_:)

Opens the specified system URL.

watchOS 2.0+

``` source
@MainActor
func openSystemURL(_ url: URL)
```

## Parameters 

`url`  

A URL that supports the `tel:` or `sms:` scheme. For information about the format of these URL schemes, see Apple URL Scheme Reference.

## Discussion

Use this method to initiate phone calls or send messages. The URL you open is sent to the appropriate system app for handling, at which point the user can choose whether to continue the operation.

