

- Core Services
- Search Kit
-  SKLoadDefaultExtractorPlugIns() 

Function

# SKLoadDefaultExtractorPlugIns()

Tells Search Kit to use the Spotlight metadata importers.

macOS 10.3+

``` source
func SKLoadDefaultExtractorPlugIns()
```

## Discussion

The Spotlight metadata importers determine the `kMDItemTextContent` property for each document passed to the SKIndexAddDocument(_:_:_:_:) function.

Call the `SKLoadDefaultExtractorPlugIns` function once at application launch to tell Search Kit to use the Spotlight metadata importers. The function SKIndexAddDocument(_:_:_:_:) will then use Spotlight’s importers to extract the text from supported files and place that text into an index, leaving the markup behind.

### Version-Notes

In versions of macOS prior to OS X v10.4, Search Kit used its own set of default text extractor plug-ins. The file types supported by Search Kit’s default text extractor plug-ins were:

- plaintext

- PDF

- HTML

- RTF

- Microsoft Word (.doc)

