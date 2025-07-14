

- Core Services
- File Metadata
- MDItem
- Audio Metadata Attribute Keys
-  kMDItemMusicalInstrumentCategory 

Global Variable

# kMDItemMusicalInstrumentCategory

Specifies the category of an instrument. A CFString.

macOS 10.4+

``` source
let kMDItemMusicalInstrumentCategory: CFString!
```

## Discussion

Files should have an instrument associated with them ("Other Instrument" is provided as a catch-all). For some categories, such as "Keyboards", there are instrument names which provide a more detailed instrument definition, for example "Piano" or "Organ".

