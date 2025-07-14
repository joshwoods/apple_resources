

- PassKit (Apple Pay and Wallet)
- Wallet
- PKAddSecureElementPassError
-  hash(into:) 

Instance Method

# hash(into:)

Hashes the Secure Element pass error object by feeding the item into the given hasher.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.5+macOS 10.10+visionOS 1.0+watchOS 2.0+Xcode 12.5+

``` source
func hash(into hasher: inout Hasher)
```

## Parameters 

`hasher`  

The hasher to use when combining the components of this instance.

## Discussion

Implement this method to conform to the Hashable protocol. The components for hashing must be the same as the compared components in your type’s `==` operator implementation. Call `hasher.combine(_:)` with each of these components.

Note

Never call `finalize()` on `hasher` because it can generate a compile-time error.

## See Also

### Hashing

var hashValue: Int

The hash value for the Secure Element pass error.

