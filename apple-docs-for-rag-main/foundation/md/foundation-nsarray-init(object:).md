

- Foundation
- NSArray
-  init(object:) 

Initializer

# init(object:)

Creates and returns an array containing a given object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init(object anObject: Any)
```

## Parameters 

`anObject`  

An object.

## Return Value

An array containing the single element `anObject`.

## Discussion

Alternatively, you can use array literal syntax in Objective-C or Swift to create an array containing a given object:

- Swift
- Objective-C

```
let array: NSArray = ["Hello, world!"]
```

```
NSArray *array = @[@"Hello, world!"];
```

## See Also

### Creating an Array

init?(contentsOfURL: URL)

Creates and returns an array containing the contents specified by a given URL.

convenience init(objects: UnsafePointer&lt;AnyObject>, count: Int)

Creates and returns an array that includes a given number of objects from a given C array.

