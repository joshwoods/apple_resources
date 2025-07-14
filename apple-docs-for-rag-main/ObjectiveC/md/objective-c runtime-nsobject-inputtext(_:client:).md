

- Objective-C Runtime
- NSObject
-  inputText(\_:client:) 

Instance Method

# inputText(\_:client:)

Handles key down events that do not map to an action method.

macOS

``` source
func inputText(
    _ string: String!,
    client sender: Any!
) -> Bool
```

## Parameters 

`string`  

The key down event, which is the text input by the client.

`sender`  

The client object sending the key down events.

## Return Value

YES if the input is accepted; otherwise NO.

## Discussion

An input method should implement this method when using key binding (that is, it implements didCommand(by:client:)).

