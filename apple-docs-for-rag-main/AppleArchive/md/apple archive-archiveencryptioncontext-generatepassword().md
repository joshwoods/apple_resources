

- Apple Archive
- ArchiveEncryptionContext
-  generatePassword() 

Instance Method

# generatePassword()

Generates a new password.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOSwatchOS 8.0+

``` source
func generatePassword() throws -> String
```

## Return Value

The new password.

## Discussion

This function generates a new high entropy password, stores it in the context, and returns it.

## See Also

### Setting a password

var password: String?

The password used to encrypt or decrypt an archive.

func setPassword(String) throws

Sets the password from the supplied string.

