

- Objective-C Runtime
- NSObject
-  inputText(\_:key:modifiers:client:) 

Instance Method

# inputText(\_:key:modifiers:client:)

Receives Unicode, the key code that generated it, and any modifier flags.

macOS

``` source
func inputText(
    _ string: String!,
    key keyCode: Int,
    modifiers flags: Int,
    client sender: Any!
) -> Bool
```

## Parameters 

`string`  

The text input by the client.

`keyCode`  

The key code for the associated Unicode.

`flags`  

The modifier flags.

`sender`  

The client object.

## Return Value

YES if the input is accepted; otherwise NO.

