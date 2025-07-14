

- Objective-C Runtime
- NSObject
-  instancesRespond(to:) 

Type Method

# instancesRespond(to:)

Returns a Boolean value that indicates whether instances of the receiver are capable of responding to a given selector.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
class func instancesRespond(to aSelector: Selector!) -> Bool
```

## Parameters 

`aSelector`  

A Selector.

## Return Value

YES if instances of the receiver are capable of responding to `aSelector` messages, otherwise NO.

## Discussion

If `aSelector` messages are forwarded to other objects, instances of the class are able to receive those messages without error even though this method returns NO.

To ask the class whether it, rather than its instances, can respond to a particular message, send to the class instead the `NSObject` protocol instance method responds(to:).

