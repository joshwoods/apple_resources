

- Core Services
- File Metadata
- MDItem
- Common Metadata Attribute Keys
-  kMDItemTextContent 

Global Variable

# kMDItemTextContent

Contains a text representation of the content of the document. Data in multiple fields should be combined using a whitespace character as a separator. A CFString.

macOS 10.4+

``` source
let kMDItemTextContent: CFString!
```

## Discussion

An application's Spotlight importer provides the content of this attribute. Applications can search for values in this attribute, but are not able to read the content of this attribute directly.

