

- App Store Connect API
- AppEncryptionDeclaration
-  AppEncryptionDeclaration.Attributes 

Object

# AppEncryptionDeclaration.Attributes

Attributes that describe an App Encryption Declarations resource.

App Store Connect API 1.0+

``` source
object AppEncryptionDeclaration.Attributes
```

## Properties

`availableOnFrenchStore`

`boolean`

A Boolean value that indicates the intent to distribute your app on the French App Store.

`codeValue`

`string`

A unique identifier that can be added to your app to associate it with a given declaration.

`containsProprietaryCryptography`

`boolean`

A Boolean value that indicates your app implements any proprietary encryption algorithms.

`containsThirdPartyCryptography`

`boolean`

A Boolean value that indicates your app implements any standard encryption algorithms instead of, or in addition to, using or accessing the encryption in Apple’s operating systems.

`documentName`

`string`

Deprecated 

The document name of your submitted export compliance documentation.

`documentType`

`string`

Deprecated 

The file type of your submitted export compliance documentation.

`documentUrl`

`string`

Deprecated 

The URL to the file of your submitted export compliance documentation.

`exempt`

`boolean`

A Boolean value that indicates your app is exempt based on your use of encryption and the app’s availability.

`platform`

Platform

The platform of the declaration.

`usesEncryption`

`boolean`

Deprecated 

A Boolean value that indicates whether your app uses, contains, or incorporates cryptography.

`appEncryptionDeclarationState`

AppEncryptionDeclarationState

The approval state of your export compliance documentation.

`uploadedDate`

`date-time`

Deprecated 

The date and time you submitted your declaration.

`appDescription`

`string`

`createdDate`

`date-time`

## See Also

### Related Documentation

App Encryption Declarations

View, and assign to builds, the declarations about types of encryption used in your app.

### Objects

object AppEncryptionDeclaration.Relationships

The relationships you included in the request and those on which you can operate.

