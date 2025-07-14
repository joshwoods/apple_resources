

- Core NFC
- NFCVASCommandConfiguration
-  init(vasMode:passTypeIdentifier:url:) 

Initializer

# init(vasMode:passTypeIdentifier:url:)

Creates a VAS command configuration object.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+

``` source
init(
    vasMode mode: NFCVASCommandConfiguration.Mode,
    passTypeIdentifier: String,
    url: URL?
)
```

## Parameters 

`mode`  

A VAS operation mode.

`passTypeIdentifier`  

A type identifier for the Wallet pass.

`url`  

A URL when `mode` is `VASModeURLOnly`; otherwise set to `nil`. The maximum length of the URL is 64 characters, including the schema.

## Return Value

A newly initialized VAS command configuration object.

