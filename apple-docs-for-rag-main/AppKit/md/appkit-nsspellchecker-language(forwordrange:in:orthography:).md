

- AppKit
- NSSpellChecker
-  language(forWordRange:in:orthography:) 

Instance Method

# language(forWordRange:in:orthography:)

macOS 10.7+

``` source
func language(
    forWordRange range: NSRange,
    in string: String,
    orthography: NSOrthography?
) -> String?
```

## See Also

### Instance Methods

func deletesAutospaceBetweenString(String, andString: String, language: String?) -> Bool

func preventsAutocorrection(before: String, language: String?) -> Bool

func requestCandidates(forSelectedRange: NSRange, in: String, types: NSTextCheckingTypes, options: [NSSpellChecker.OptionKey : Any]?, inSpellDocumentWithTag: Int, completionHandler: ((Int, [NSTextCheckingResult]) -> Void)?) -> Int

func showInlinePrediction(forCandidates: [NSTextCheckingResult], client: any NSTextInputClient)

