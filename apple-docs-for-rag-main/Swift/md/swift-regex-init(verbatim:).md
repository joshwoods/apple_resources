

- Swift
- Regex
-  init(verbatim:) 

Initializer

# init(verbatim:)

Creates a regular expression that matches the given string exactly, as though every metacharacter in it was escaped.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(verbatim verbatimString: String)
```

## Parameters 

`verbatimString`  

A string to convert into a regular expression exactly, escaping any metacharacters.

## Discussion

This example creates a regular expression that matches the string `"(adj)"`, including the parentheses. Although parentheses are regular expression metacharacters, they do not need escaping in the string passed as `verbatimString`.

```
let adjectiveDesignator = Regex(verbatim: "(adj.)")

print("awesome (adj.)".contains(adjectiveDesignator))
// Prints "true"
print("apple (n.)".contains(adjectiveDesignator))
// Prints "false"
```

