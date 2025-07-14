

- AppKit
- NSSpellChecker
-  deletesAutospaceBetweenString(\_:andString:language:) 

Instance Method

# deletesAutospaceBetweenString(\_:andString:language:)

macOS 10.12.2+

``` source
func deletesAutospaceBetweenString(
    _ precedingString: String,
    andString followingString: String,
    language: String?
) -> Bool
```

## See Also

### Instance Methods

func language(forWordRange: NSRange, in: String, orthography: NSOrthography?) -> String?

func preventsAutocorrection(before: String, language: String?) -> Bool

func requestCandidates(forSelectedRange: NSRange, in: String, types: NSTextCheckingTypes, options: [NSSpellChecker.OptionKey : Any]?, inSpellDocumentWithTag: Int, completionHandler: ((Int, [NSTextCheckingResult]) -> Void)?) -> Int

func showInlinePrediction(forCandidates: [NSTextCheckingResult], client: any NSTextInputClient)

