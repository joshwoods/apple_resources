

- Combine
- Subscriber
-  Failure 

Associated Type

# Failure

The kind of errors this subscriber might receive.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
associatedtype Failure : Error
```

**Required**

## Discussion

Use `Never` if this `Subscriber` cannot receive errors.

## See Also

### Declaring Subscriber Topography

associatedtype Input

The kind of values this subscriber receives.

**Required**

