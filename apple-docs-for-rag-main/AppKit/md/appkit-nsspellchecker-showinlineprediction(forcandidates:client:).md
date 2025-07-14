

- AppKit
- NSSpellChecker
-  showInlinePrediction(forCandidates:client:) 

Instance Method

# showInlinePrediction(forCandidates:client:)

macOS 14.0+

``` source
func showInlinePrediction(
    forCandidates candidates: [NSTextCheckingResult],
    client: any NSTextInputClient
)
```

## See Also

### Instance Methods

func deletesAutospaceBetweenString(String, andString: String, language: String?) -> Bool

func language(forWordRange: NSRange, in: String, orthography: NSOrthography?) -> String?

func preventsAutocorrection(before: String, language: String?) -> Bool

func requestCandidates(forSelectedRange: NSRange, in: String, types: NSTextCheckingTypes, options: [NSSpellChecker.OptionKey : Any]?, inSpellDocumentWithTag: Int, completionHandler: ((Int, [NSTextCheckingResult]) -> Void)?) -> Int

