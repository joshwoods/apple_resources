

- StoreKit
- Product
-  jsonRepresentation 

Instance Property

# jsonRepresentation

The JSON representation of the product information.

iOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var jsonRepresentation: Data { get }
```

## Discussion

The jsonRepresentation is UTF-8 string data. You can use the JSON data to decode the product information into your own data type instead of using the Product value directly.

