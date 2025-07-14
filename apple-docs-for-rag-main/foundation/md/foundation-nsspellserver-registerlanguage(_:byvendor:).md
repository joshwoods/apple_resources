

- Foundation
- NSSpellServer
-  registerLanguage(\_:byVendor:) 

Instance Method

# registerLanguage(\_:byVendor:)

Notifies the receiver of a language your spelling checker can check.

Mac Catalyst 13.0+macOS 10.0+

``` source
func registerLanguage(
    _ language: String?,
    byVendor vendor: String?
) -> Bool
```

## Parameters 

`language`  

A string specifying the English name of a language on Apple’s list of languages.

`vendor`  

A string that identifies the vendor (to distinguish your spelling checker from those that others may offer for the same language).

## Return Value

Returns true if the language is registered, false if for some reason it can’t be registered.

## Discussion

If your spelling checker supports more than one language, it should invoke this method once for each language. Registering a language-vendor combination causes it to appear in the Spelling panel’s pop-up menu of spelling checkers.

## See Also

### Providing Spelling Services

func run()

Causes the receiver to start listening for spell-checking requests.

