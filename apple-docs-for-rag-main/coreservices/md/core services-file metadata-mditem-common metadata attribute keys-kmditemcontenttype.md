

- Core Services
- File Metadata
- MDItem
- Common Metadata Attribute Keys
-  kMDItemContentType 

Global Variable

# kMDItemContentType

The UTI pedigree of a file. A CFString.

macOS 10.4+

``` source
let kMDItemContentType: CFString!
```

## Discussion

For example, a jpeg image file will have a value of public.jpeg/public.image/public.data. The value of this attribute is set by the MDImporter. Changes to this value are lost when the file attributes are next imported.

