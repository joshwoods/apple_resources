

- Swift
- StringProtocol
-  localizedStandardContains(\_:) 

Instance Method

# localizedStandardContains(\_:)

Returns a Boolean value indicating whether the string contains the given string, taking the current locale into account.

iOS 9.0+iPadOS 9.0+Mac Catalyst 9.0+macOS 10.11+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func localizedStandardContains(_ string: T) -> Bool where T : StringProtocol
```

## Discussion

This is the most appropriate method for doing user-level string searches, similar to how searches are done generally in the system. The search is locale-aware, case and diacritic insensitive. The exact list of search options applied may change over time.

