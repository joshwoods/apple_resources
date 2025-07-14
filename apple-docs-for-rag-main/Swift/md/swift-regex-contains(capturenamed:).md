

- Swift
- Regex
-  contains(captureNamed:) 

Instance Method

# contains(captureNamed:)

Returns a Boolean value indicating whether a named capture with the given name exists.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func contains(captureNamed name: String) -> Bool
```

## Parameters 

`name`  

The name to look for among the regular expression’s capture groups. Capture group names are case sensitive.

## Discussion

This example shows a regular expression that includes capture groups named `key` and `value`:

```
let regex = try Regex("(?'key'.+?): (?'value'.+)")
regex.contains(captureNamed: "key")       // true
regex.contains(captureNamed: "VALUE")     // false
regex.contains(captureNamed: "1")         // false
```

