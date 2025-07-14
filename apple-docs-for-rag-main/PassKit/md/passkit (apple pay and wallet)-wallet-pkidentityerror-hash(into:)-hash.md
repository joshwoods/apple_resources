

- PassKit (Apple Pay and Wallet)
- Wallet
- PKIdentityError
-  hash(into:) 

Instance Method

# hash(into:)

Hashes the essential components of the value by passing them into the hasher.

iOS 8.0+iPadOS 8.0+Mac Catalyst 16.0+visionOS 1.0+watchOS 2.0+Xcode 7.2+

``` source
func hash(into hasher: inout Hasher)
```

## Parameters 

`hasher`  

The hasher to use when combining the components of this instance.

## See Also

### Accessing the hash value

var hashValue: Int

The hash value.

