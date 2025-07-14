

- UIKit
- UIPasteboard
-  setItemProviders(\_:localOnly:expirationDate:) 

Instance Method

# setItemProviders(\_:localOnly:expirationDate:)

Sets and configures an explicit array of item providers for the pasteboard.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
func setItemProviders(
    _ itemProviders: [NSItemProvider],
    localOnly: Bool,
    expirationDate: Date?
)
```

## Parameters 

`itemProviders`  

An array of item providers for the pasteboard.

`localOnly`  

If false, the pasteboard items are available to other devices through the Handoff feature; if true, the pasteboard items are only available to the local device.

`expirationDate`  

An NSDate value that specifies the time and date that you want the system to remove the pasteboard items from the pasteboard.

## See Also

### Getting and setting item providers

var itemProviders: [NSItemProvider]

An array of item providers for the pasteboard.

func setObjects([any NSItemProviderWriting])

Sets an array of item providers for the pasteboard, based on a specified array of objects.

func setObjects&lt;T>([T])

Sets an array of item providers for the pasteboard, based on a specified array of objects.

func setObjects([any NSItemProviderWriting], localOnly: Bool, expirationDate: Date?)

Sets and configures an array of item providers for the pasteboard, based on a specified array of objects.

func setObjects&lt;T>([T], localOnly: Bool, expirationDate: Date?)

Sets and configures an array of item providers for the pasteboard, based on a specified array of objects.

