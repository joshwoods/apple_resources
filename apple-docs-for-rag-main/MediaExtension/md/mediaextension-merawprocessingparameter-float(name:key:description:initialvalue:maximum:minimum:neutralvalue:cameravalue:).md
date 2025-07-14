

- MediaExtension
- MERAWProcessingParameter
-  float(name:key:description:initialValue:maximum:minimum:neutralValue:cameraValue:) 

Type Method

# float(name:key:description:initialValue:maximum:minimum:neutralValue:cameraValue:)

macOS 15.0+

``` source
class func float(
    name: String,
    key: String,
    description: String,
    initialValue: Float,
    maximum: Float,
    minimum: Float,
    neutralValue: Float?,
    cameraValue: Float?
) -> MERAWProcessingParameter.FloatingPoint
```

## See Also

### Class methods

class func boolean(name: String, key: String, description: String, initialValue: Bool, neutralValue: Bool?, cameraValue: Bool?) -> MERAWProcessingParameter.Boolean

class func integer(name: String, key: String, description: String, initialValue: Int, maximum: Int, minimum: Int, neutralValue: Int?, cameraValue: Int?) -> MERAWProcessingParameter.Integer

class func list(name: String, key: String, description: String, list: [MERAWProcessingParameter.ListElement], initialValue: Int, neutralValue: Int?, cameraValue: Int?) -> MERAWProcessingParameter.List

class func listElement(name: String, description: String, elementID: Int) -> MERAWProcessingParameter.ListElement

class func subGroup(name: String, description: String, parameters: [MERAWProcessingParameter]) -> MERAWProcessingParameter.SubGroup

