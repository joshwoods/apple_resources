

- HomeKit
- HMNumberRange
-  init(minValue:) 

Initializer

# init(minValue:)

Creates an one-sided number range with a minimum value.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+tvOS 11.0+visionOS 1.0+watchOS 4.0+

``` source
convenience init(minValue: NSNumber)
```

## Parameters 

`minValue`  

The minimum value of the range.

## Return Value

An initialized number range, with the maximum value set to an arbitrarily large value.

## See Also

### Creating a number range

convenience init(minValue: NSNumber, maxValue: NSNumber)

Creates a new number range.

convenience init(maxValue: NSNumber)

Creates a one-sided number range with a maximum value.

