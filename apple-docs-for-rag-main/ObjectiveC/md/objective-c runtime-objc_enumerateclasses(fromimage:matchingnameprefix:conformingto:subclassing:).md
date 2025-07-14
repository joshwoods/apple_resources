

- Objective-C Runtime
-  objc_enumerateClasses(fromImage:matchingNamePrefix:conformingTo:subclassing:) 

Function

# objc_enumerateClasses(fromImage:matchingNamePrefix:conformingTo:subclassing:)

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
func objc_enumerateClasses(
    fromImage: ObjCEnumerationImage = .machHeader(#dsohandle),
    matchingNamePrefix: String? = nil,
    conformingTo: Protocol? = nil,
    subclassing: AnyClass? = nil
) -> ObjCClassList
```

## See Also

### Functions

func autoreleasepool&lt;E, Result>(invoking: () throws(E) -> Result) throws(E) -> Result

func class_lookupMethod(AnyClass?, Selector) -> IMP?Deprecated

func class_respondsToMethod(AnyClass?, Selector) -> BoolDeprecated

func objc_addExceptionHandler(objc_exception_handler, UnsafeMutableRawPointer?) -> UInt

func objc_addLoadImageFunc(objc_func_loadImage)

func objc_assertRegisteredThreadWithCollector()Deprecated

func objc_begin_catch(UnsafeMutableRawPointer) -> Any

func objc_clear_stack(UInt)Deprecated

func objc_collect(UInt)Deprecated

func objc_collectableZone() -> objc_zone_t!Deprecated

func objc_collecting_enabled() -> BoolDeprecated

func objc_collectingEnabled() -> BoolDeprecated

func objc_end_catch()

func objc_exception_rethrow() -> Never

func objc_exception_throw(Any) -> Never

Throw a runtime exception. This function is inserted by the compiler where \c @throw would otherwise be.

