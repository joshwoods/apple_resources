

- HomeKit
- HMNumberRange
-  init(maxValue:) 

Initializer

# init(maxValue:)

Creates a one-sided number range with a maximum value.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
convenience init(maxValue: NSNumber)
```

## Parameters 

`maxValue`  

The maximum value of the range.

## Return Value

An initialized number range, with the minimum value set to an arbitrarily large negative value.

## See Also

### Creating a number range

convenience init(minValue: NSNumber, maxValue: NSNumber)

Creates a new number range.

convenience init(minValue: NSNumber)

Creates an one-sided number range with a minimum value.

