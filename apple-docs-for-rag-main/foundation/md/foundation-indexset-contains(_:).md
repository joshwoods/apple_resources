

- Foundation
- IndexSet
-  contains(\_:) 

Instance Method

# contains(\_:)

Returns `true` if `self` contains `integer`.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func contains(_ integer: IndexSet.Element) -> Bool
```

## See Also

### Testing Set Membership

func contains(integersIn: IndexSet) -> Bool

Returns `true` if `self` contains all of the integers in `indexSet`.

func contains(integersIn: Range&lt;IndexSet.Element>) -> Bool

Returns `true` if `self` contains all of the integers in `range`.

func intersects(integersIn: Range&lt;IndexSet.Element>) -> Bool

Returns `true` if `self` intersects any of the integers in `range`.

