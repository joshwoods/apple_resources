

- Foundation
- NSArray
-  componentsJoined(by:) 

Instance Method

# componentsJoined(by:)

Constructs and returns an `NSString` object that is the result of interposing a given separator between the elements of the array.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func componentsJoined(by separator: String) -> String
```

## Parameters 

`separator`  

The string to interpose between the elements of the array.

## Return Value

An `NSString` object that is the result of interposing `separator` between the elements of the array. If the array has no elements, returns an `NSString` object representing an empty string.

## Discussion

For example, this code excerpt writes “`here be dragons`” to the console:

```
NSArray *pathArray = [NSArray arrayWithObjects:@"here", @"be", @"dragons", nil];
NSLog(@"%@",[pathArray componentsJoinedByString:@" "]);
```

### Special Considerations

Each element in the array must handle `description`.

## See Also

### Related Documentation

func components(separatedBy: String) -> [String]

Returns an array containing substrings from the receiver that have been divided by a given separator.

