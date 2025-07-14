

- RegexBuilder
- ChoiceOf
-  init(\_:) 

Initializer

# init(\_:)

Creates a regex component that chooses exactly one of the regex components provided by the builder closure.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
init(@AlternationBuilder _ builder: () -> ChoiceOf)
```

## Parameters 

`builder`  

A builder closure that declares a list of regex components, each of which can be exclusively matched.

## Discussion

In this example, `regex` successfully matches either a `"CREDIT"` or `"DEBIT"` substring:

```
let regex = Regex {
    ChoiceOf {
        "CREDIT"
        "DEBIT"
    }
}
let match = try regex.prefixMatch(in: "DEBIT    04032020    Payroll $69.73")
print(match?.0 as Any)
// Prints "DEBIT"
```

