

- Bundle Resources
- Information Property List
-  ATSApplicationFontsPath 

Property List Key

# ATSApplicationFontsPath

The location of a font file or folder of fonts in the bundle’s Resources folder.

macOS 10.0+

## Details 

Name  
Application fonts resource path

Type  

string

## Discussion

If you set this key, the system allows the app in the bundle to use the fonts at the specified path. Set this key to the path relative to the bundle’s `Resources` folder. For example, if the fonts are in `.../Resources/MyFonts`, set this key to `MyFonts/`.

## See Also

### Fonts

UIAppFonts

App-specific font files located in the bundle and that the system loads at runtime.

**Name:** Fonts provided by application

