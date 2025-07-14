

- UIKit
- UIPasteboard
-  setObjects(\_:) 

Instance Method

# setObjects(\_:)

Sets an array of item providers for the pasteboard, based on a specified array of objects.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
func setObjects(_ objects: [any NSItemProviderWriting])
```

## Parameters 

`objects`  

An array of item providers for the pasteboard.

## See Also

### Getting and setting item providers

var itemProviders: [NSItemProvider]

An array of item providers for the pasteboard.

func setItemProviders([NSItemProvider], localOnly: Bool, expirationDate: Date?)

Sets and configures an explicit array of item providers for the pasteboard.

func setObjects&lt;T>([T])

Sets an array of item providers for the pasteboard, based on a specified array of objects.

func setObjects([any NSItemProviderWriting], localOnly: Bool, expirationDate: Date?)

Sets and configures an array of item providers for the pasteboard, based on a specified array of objects.

func setObjects&lt;T>([T], localOnly: Bool, expirationDate: Date?)

Sets and configures an array of item providers for the pasteboard, based on a specified array of objects.

