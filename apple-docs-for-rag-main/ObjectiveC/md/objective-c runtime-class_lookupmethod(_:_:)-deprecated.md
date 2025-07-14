

- Objective-C Runtime
-  class_lookupMethod(\_:\_:) Deprecated

Function

# class_lookupMethod(\_:\_:)

tvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 1.0–1.0Deprecated

``` source
func class_lookupMethod(
    _ cls: AnyClass?,
    _ sel: Selector
) -> IMP?
```

Deprecated

use class_getMethodImplementation instead

## See Also

### Functions

func autoreleasepool&lt;E, Result>(invoking: () throws(E) -> Result) throws(E) -> Result

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

func objc_enumerateClasses(fromImage: ObjCEnumerationImage, matchingNamePrefix: String?, conformingTo: Protocol?, subclassing: AnyClass?) -> ObjCClassList

func objc_exception_rethrow() -> Never

func objc_exception_throw(Any) -> Never

Throw a runtime exception. This function is inserted by the compiler where \c @throw would otherwise be.

