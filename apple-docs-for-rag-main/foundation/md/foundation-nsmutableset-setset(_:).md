

- Foundation
- NSMutableSet
-  setSet(\_:) 

Instance Method

# setSet(\_:)

Empties the receiving set, then adds each object contained in another given set.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func setSet(_ otherSet: Set)
```

## Parameters 

`otherSet`  

The set whose members replace the receiving set’s content.

## See Also

### Combining and recombining sets

func union(Set&lt;AnyHashable>)

Adds each object in another given set to the receiving set, if not present.

func minus(Set&lt;AnyHashable>)

Removes each object in another given set from the receiving set, if present.

func intersect(Set&lt;AnyHashable>)

Removes from the receiving set each object that isn’t a member of another given set.

