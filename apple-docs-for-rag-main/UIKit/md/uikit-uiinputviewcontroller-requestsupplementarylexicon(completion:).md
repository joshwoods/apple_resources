

- UIKit
- UIInputViewController
-  requestSupplementaryLexicon(completion:) 

Instance Method

# requestSupplementaryLexicon(completion:)

Obtains a supplementary lexicon of term pairs in a custom keyboard.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
func requestSupplementaryLexicon(completion completionHandler: @escaping (UILexicon) -> Void)
```

``` source
@MainActor
func requestSupplementaryLexicon() async -> UILexicon
```

## Parameters 

`completionHandler`  

Code that you write to make use of the returned `UILexicon` object.

## Discussion

Call this method to obtain a UILexicon object containing a basic set of term pairs for use in autocorrection or textual suggestions based on user input. The UILexicon object contains words from various sources, including:

- Unpaired first names and last names from the user’s Address Book database

- Text shortcuts defined in the Settings \> General \> Keyboard \> Shortcuts list

- A common words dictionary

Consider this lexicon as a supplement to a more complete lexicon of your own design.

