

- PassKit (Apple Pay and Wallet)
- Wallet
- PKAddSecureElementPassError
-  hashValue 

Instance Property

# hashValue

The hash value for the Secure Element pass error.

iOS 8.0+iPadOS 8.0+Mac Catalyst 14.5+macOS 10.10+visionOS 1.0+watchOS 2.0+Xcode 12.5+

``` source
var hashValue: Int { get }
```

## Discussion

Because hash values aren’t always equal across app executions, saving them for future execution isn’t reliable.

Important

`hashValue` is deprecated as a Hashable requirement. To conform to `Hashable`, implement the hash(into:) requirement instead.

## See Also

### Hashing

func hash(into: inout Hasher)

Hashes the Secure Element pass error object by feeding the item into the given hasher.

