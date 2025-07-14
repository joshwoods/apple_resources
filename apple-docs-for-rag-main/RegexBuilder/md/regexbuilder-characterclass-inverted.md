

- RegexBuilder
- CharacterClass
-  inverted 

Instance Property

# inverted

A character class that matches any character that does not match this character class.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
var inverted: CharacterClass { get }
```

## Discussion

For example, you can use the `inverted` property to create a character class that excludes a specific group of characters:

```
let validCharacters = CharacterClass("a"..."z", .anyOf("-_"))
let invalidCharacters = validCharacters.inverted

let username = "user123"
if username.contains(invalidCharacters) {
    print("Invalid username: '\(username)'")
}
// Prints "Invalid username: 'user123'"
```

