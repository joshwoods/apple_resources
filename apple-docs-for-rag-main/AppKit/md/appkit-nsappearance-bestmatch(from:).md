

- AppKit
- NSAppearance
-  bestMatch(from:) 

Instance Method

# bestMatch(from:)

Returns the appearance name that most closely matches the current appearance object.

macOS 10.14+

``` source
func bestMatch(from appearances: [NSAppearance.Name]) -> NSAppearance.Name?
```

## Parameters 

`appearances`  

An array of appearance names, representing the appearances that your app supports.

## Return Value

The name of the appearance that most closely matches the current appearance object.

## Discussion

You can use this method in situations where your app doesn’t fully support the current appearance, but supports a different appearance object that has similar qualities. This method returns the name from the `appearances` array that comes closest to matching the current appearance object’s attributes.

