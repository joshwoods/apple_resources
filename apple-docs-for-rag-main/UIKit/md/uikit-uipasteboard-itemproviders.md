

- UIKit
- UIPasteboard
-  itemProviders 

Instance Property

# itemProviders

An array of item providers for the pasteboard.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
var itemProviders: [NSItemProvider] { get set }
```

## See Also

### Getting and setting item providers

func setItemProviders([NSItemProvider], localOnly: Bool, expirationDate: Date?)

Sets and configures an explicit array of item providers for the pasteboard.

func setObjects([any NSItemProviderWriting])

Sets an array of item providers for the pasteboard, based on a specified array of objects.

func setObjects&lt;T>([T])

Sets an array of item providers for the pasteboard, based on a specified array of objects.

func setObjects([any NSItemProviderWriting], localOnly: Bool, expirationDate: Date?)

Sets and configures an array of item providers for the pasteboard, based on a specified array of objects.

func setObjects&lt;T>([T], localOnly: Bool, expirationDate: Date?)

Sets and configures an array of item providers for the pasteboard, based on a specified array of objects.

