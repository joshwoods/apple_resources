

- Objective-C Runtime
- NSObject
-  saveOptions(\_:shouldShowUTType:) 

Instance Method

# saveOptions(\_:shouldShowUTType:)

Called to determine if the specified uniform type identifier should be shown in the save panel.

macOS 10.6+

``` source
func saveOptions(
    _ saveOptions: IKSaveOptions!,
    shouldShowUTType utType: String!
) -> Bool
```

## Parameters 

`saveOptions`  

The `IKSaveOptions` instance that called the delegate.

`utType`  

The uniform type identifier to test.

## Return Value

YES if the specified type should be shown in the save options, otherwise NO.

