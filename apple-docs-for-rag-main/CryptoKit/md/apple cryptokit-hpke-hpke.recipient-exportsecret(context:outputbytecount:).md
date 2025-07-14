

- Apple CryptoKit
- HPKE
- HPKE.Recipient
-  exportSecret(context:outputByteCount:) 

Instance Method

# exportSecret(context:outputByteCount:)

Exports a secret given domain-separation context and the desired output length.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func exportSecret(
    context: Context,
    outputByteCount: Int
) throws -> SymmetricKey where Context : DataProtocol
```

## Parameters 

`context`  

Application-specific information providing context on the use of this key.

`outputByteCount`  

The desired length of the exported secret.

## Return Value

The exported secret.

