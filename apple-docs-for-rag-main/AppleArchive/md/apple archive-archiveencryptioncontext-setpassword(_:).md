

- Apple Archive
- ArchiveEncryptionContext
-  setPassword(\_:) 

Instance Method

# setPassword(\_:)

Sets the password from the supplied string.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
func setPassword(_ password: String) throws
```

## Parameters 

`password`  

The password.

## Discussion

Use this function to encrypt or decrypt an archive with the scrypt encryption mode.

## See Also

### Setting a password

var password: String?

The password used to encrypt or decrypt an archive.

func generatePassword() throws -> String

Generates a new password.

