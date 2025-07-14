

- Apple Archive
- ArchiveEncryptionContext
-  password 

Instance Property

# password

The password used to encrypt or decrypt an archive.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
var password: String? { get set }
```

## Discussion

Use the generatePassword() function to generate random high entropy passwords.

## See Also

### Setting a password

func generatePassword() throws -> String

Generates a new password.

func setPassword(String) throws

Sets the password from the supplied string.

