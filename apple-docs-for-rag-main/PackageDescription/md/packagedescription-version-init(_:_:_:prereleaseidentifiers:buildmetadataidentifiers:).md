

- PackageDescription
- Version
-  init(\_:\_:\_:prereleaseIdentifiers:buildMetadataIdentifiers:) 

Initializer

# init(\_:\_:\_:prereleaseIdentifiers:buildMetadataIdentifiers:)

Initializes a version struct with the provided components of a semantic version.

``` source
init(
    _ major: Int,
    _ minor: Int,
    _ patch: Int,
    prereleaseIdentifiers: [String] = [],
    buildMetadataIdentifiers: [String] = []
)
```

## Parameters 

`major`  

The major version number.

`minor`  

The minor version number.

`patch`  

The patch version number.

`prereleaseIdentifiers`  

The pre-release identifier.

## Discussion

Precondition

`major >= 0 && minor >= 0 && patch >= 0`.

Precondition

`prereleaseIdentifiers` can contain only ASCII alpha-numeric characters and “-”.

Precondition

`buildMetaDataIdentifiers` can contain only ASCII alpha-numeric characters and “-”.

