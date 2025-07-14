

- Authentication Services
- ASImportableCredential
- ASImportableCredential.BasicAuthentication
-  init(urls:username:password:) 

Initializer

# init(urls:username:password:)

Creates a basic authentication password instance.

iOS 18.2+iPadOS 18.2+Mac Catalyst 18.2+macOS 15.2+visionOS 2.2+

``` source
init(
    urls: [String],
    username: ASImportableEditableField? = nil,
    password: ASImportableEditableField? = nil
)
```

## Parameters 

`urls`  

The list of URLs for which to fill the password.

`username`  

The username associated with the credential.

`password`  

The password associated with the credential.

