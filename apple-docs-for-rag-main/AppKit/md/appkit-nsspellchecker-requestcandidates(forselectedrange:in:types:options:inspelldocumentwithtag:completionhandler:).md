

- AppKit
- NSSpellChecker
-  requestCandidates(forSelectedRange:in:types:options:inSpellDocumentWithTag:completionHandler:) 

Instance Method

# requestCandidates(forSelectedRange:in:types:options:inSpellDocumentWithTag:completionHandler:)

macOS 10.12.2+

``` source
func requestCandidates(
    forSelectedRange selectedRange: NSRange,
    in stringToCheck: String,
    types checkingTypes: NSTextCheckingTypes,
    options: [NSSpellChecker.OptionKey : Any]? = nil,
    inSpellDocumentWithTag tag: Int,
    completionHandler: ((Int, [NSTextCheckingResult]) -> Void)? = nil
) -> Int
```

## See Also

### Instance Methods

func deletesAutospaceBetweenString(String, andString: String, language: String?) -> Bool

func language(forWordRange: NSRange, in: String, orthography: NSOrthography?) -> String?

func preventsAutocorrection(before: String, language: String?) -> Bool

func showInlinePrediction(forCandidates: [NSTextCheckingResult], client: any NSTextInputClient)

