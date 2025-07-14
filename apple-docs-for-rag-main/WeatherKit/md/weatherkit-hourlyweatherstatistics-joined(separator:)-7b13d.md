

- WeatherKit
- HourlyWeatherStatistics
-  joined(separator:) 

Instance Method

# joined(separator:)

Returns a new string by concatenating the elements of the sequence, adding the given separator between each element.

WeatherKitSwiftiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func joined(separator: String = "") -> String
```

Available when `Element` conforms to `StringProtocol`.

## Parameters 

`separator`  

A string to insert between each of the elements in this sequence. The default separator is an empty string.

## Return Value

A single, concatenated string.

## Discussion

The following example shows how an array of strings can be joined to a single, comma-separated string:

```
let cast = ["Vivien", "Marlon", "Kim", "Karl"]
let list = cast.joined(separator: ", ")
print(list)
// Prints "Vivien, Marlon, Kim, Karl"
```

