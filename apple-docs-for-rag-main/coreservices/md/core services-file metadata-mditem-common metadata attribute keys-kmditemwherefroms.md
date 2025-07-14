

- Core Services
- File Metadata
- MDItem
- Common Metadata Attribute Keys
-  kMDItemWhereFroms 

Global Variable

# kMDItemWhereFroms

Describes where the file was obtained from. A CFArray of CFStrings.

macOS 10.4+

``` source
let kMDItemWhereFroms: CFString!
```

## Discussion

For example, a downloaded file may refer to the URL, files received by email may indicate the sender’s email address, message subject, etc.

