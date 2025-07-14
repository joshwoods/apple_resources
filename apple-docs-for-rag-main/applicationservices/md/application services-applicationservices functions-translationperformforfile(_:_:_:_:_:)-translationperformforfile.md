

- Application Services
- ApplicationServices Functions
-  TranslationPerformForFile(\_:\_:\_:\_:\_:) 

Function

# TranslationPerformForFile(\_:\_:\_:\_:\_:)

macOS 10.3+

``` source
func TranslationPerformForFile(
    _ inTranslation: Translation!,
    _ inSourceFile: UnsafePointer!,
    _ inDestinationDirectory: UnsafePointer!,
    _ inDestinationName: CFString!,
    _ outTranslatedFile: UnsafeMutablePointer!
) -> OSStatus
```

