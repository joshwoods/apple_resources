

- Swift Charts
-  PlottableProjection 

Structure

# PlottableProjection

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+tvOS 18.0+visionOS 2.0+watchOS 11.0+

``` source
struct PlottableProjection where DataValue : Plottable
```

## Topics

### Type Methods

static func value(LocalizedStringKey, DataValue) -> PlottableProjection&lt;DataElement, DataValue>

static func value(LocalizedStringKey, KeyPath&lt;DataElement, DataValue>) -> PlottableProjection&lt;DataElement, DataValue>

static func value(some StringProtocol, DataValue) -> PlottableProjection&lt;DataElement, DataValue>

static func value(some StringProtocol, KeyPath&lt;DataElement, DataValue>) -> PlottableProjection&lt;DataElement, DataValue>

static func value(Text, KeyPath&lt;DataElement, DataValue>) -> PlottableProjection&lt;DataElement, DataValue>

static func value(Text, DataValue) -> PlottableProjection&lt;DataElement, DataValue>

static func value(LocalizedStringKey, DataValue, DataValue) -> PlottableProjection&lt;DataElement, DataValue>

static func value(some StringProtocol, DataValue, DataValue) -> PlottableProjection&lt;DataElement, DataValue>

static func value(Text, DataValue, DataValue) -> PlottableProjection&lt;DataElement, DataValue>

static func value(Text, KeyPath&lt;DataElement, DataValue>, KeyPath&lt;DataElement, DataValue>) -> PlottableProjection&lt;DataElement, DataValue>

static func value(some StringProtocol, KeyPath&lt;DataElement, DataValue>, KeyPath&lt;DataElement, DataValue>) -> PlottableProjection&lt;DataElement, DataValue>

static func value(LocalizedStringKey, KeyPath&lt;DataElement, DataValue>, KeyPath&lt;DataElement, DataValue>) -> PlottableProjection&lt;DataElement, DataValue>

static func value(LocalizedStringKey, DataValue, unit: Calendar.Component, calendar: Calendar?) -> PlottableProjection&lt;DataElement, DataValue>

static func value(Text, KeyPath&lt;DataElement, DataValue>, unit: Calendar.Component, calendar: Calendar?) -> PlottableProjection&lt;DataElement, DataValue>

static func value(LocalizedStringKey, KeyPath&lt;DataElement, DataValue>, unit: Calendar.Component, calendar: Calendar?) -> PlottableProjection&lt;DataElement, DataValue>

static func value(some StringProtocol, DataValue, unit: Calendar.Component, calendar: Calendar?) -> PlottableProjection&lt;DataElement, DataValue>

static func value(some StringProtocol, KeyPath&lt;DataElement, DataValue>, unit: Calendar.Component, calendar: Calendar?) -> PlottableProjection&lt;DataElement, DataValue>

static func value(Text, DataValue, unit: Calendar.Component, calendar: Calendar?) -> PlottableProjection&lt;DataElement, DataValue>

