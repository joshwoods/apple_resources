

- AppKit
- NSSpellChecker
-  preventsAutocorrection(before:language:) 

Instance Method

# preventsAutocorrection(before:language:)

macOS 10.12+

``` source
func preventsAutocorrection(
    before string: String,
    language: String?
) -> Bool
```

## See Also

### Instance Methods

func deletesAutospaceBetweenString(String, andString: String, language: String?) -> Bool

func language(forWordRange: NSRange, in: String, orthography: NSOrthography?) -> String?

func requestCandidates(forSelectedRange: NSRange, in: String, types: NSTextCheckingTypes, options: [NSSpellChecker.OptionKey : Any]?, inSpellDocumentWithTag: Int, completionHandler: ((Int, [NSTextCheckingResult]) -> Void)?) -> Int

func showInlinePrediction(forCandidates: [NSTextCheckingResult], client: any NSTextInputClient)

