

- Safari Services
- SFSafariPage
-  dispatchMessageToScript(withName:userInfo:) 

Instance Method

# dispatchMessageToScript(withName:userInfo:)

Dispatches a message from the app extension to the content script injected in this page.

macOS 10.12+

``` source
func dispatchMessageToScript(
    withName messageName: String,
    userInfo: [String : Any]? = nil
)
```

## Parameters 

`messageName`  

A string that identifies the message.

`userInfo`  

An optional dictionary containing additional message content. If a dictionary is provided, values must conform to the W3C standard for safe passing of structured data, such as Boolean objects, numeric values, strings, and arrays.

## Mentioned in 

Passing messages between Safari app extensions and injected scripts

Adjusting settings for contextual menu items

