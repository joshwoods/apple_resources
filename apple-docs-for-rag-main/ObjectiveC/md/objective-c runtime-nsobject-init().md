

- Objective-C Runtime
- NSObject
-  init() 

Initializer

# init()

Implemented by subclasses to initialize a new object (the receiver) immediately after memory for it has been allocated.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
init()
```

## Return Value

An initialized object, or `nil` if an object could not be created for some reason that would not result in an exception.

## Discussion

An init() message is coupled with an alloc (or allocWithZone:) message in the same line of code:

```
SomeClass *object = [[SomeClass alloc] init];
```

An object isn’t ready to be used until it has been initialized.

In a custom implementation of this method, you must invoke super’s Initialization then initialize and return the new object. If the new object can’t be initialized, the method should return `nil`. For example, a hypothetical `BuiltInCamera` class might return `nil` from its `init` method if run on a device that has no camera.

```
- (instancetype)init {
    if (self = [super init]) {
        // Initialize self
    }
    return self;
}
```

In some cases, a custom implementation of the init() method might return a substitute object. You must therefore always use the object returned by init(), and not the one returned by alloc or allocWithZone:, in subsequent code.

The init() method defined in the `NSObject` class does no initialization; it simply returns `self`. In terms of nullability, callers can assume that the `NSObject` implementation of init() does not return `nil`.

## See Also

### Creating, Copying, and Deallocating Objects

func copy() -> Any

Returns the object returned by `copy(with:)`.

func mutableCopy() -> Any

Returns the object returned by `mutableCopy(with:)` where the zone is `nil`.

