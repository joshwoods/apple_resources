

- Core Image
- CIFilter
-  User Interface Control Options 

API Collection

# User Interface Control Options

Sets of controls for various user scenarios.

## Overview

You can use these constants to specify the controls that you want associated with each user scenario. For example, for a filter that has many input parameters you can choose a small set of input parameters that the typical consumer can control and set the other input parameters to default values. For the same filter, however, you can choose to allow professional customers to control all the input parameters.

## Topics

### Constants

let kCIUIParameterSet: String

The set of input parameters to use. The associated value can be kCIUISetBasic, kCIUISetIntermediate, kCIUISetAdvanced, or kCIUISetDevelopment.

let kCIUISetBasic: String

Controls that are appropriate for a basic user scenario, that is, the minimum of settings to control the filter.

let kCIUISetIntermediate: String

Controls that are appropriate for an intermediate user scenario.

let kCIUISetAdvanced: String

Controls that are appropriate for an advanced user scenario.

let kCIUISetDevelopment: String

Controls that should be visible only for development purposes.

