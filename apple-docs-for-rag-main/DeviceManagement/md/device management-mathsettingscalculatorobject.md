

- Device Management
-  MathSettingsCalculatorObject 

Object

# MathSettingsCalculatorObject

The declaration to configure the calculator app.

iOS 18.0+iPadOS 18.0+macOS 15.0+Device Assignment ServicesVPP License Management

``` source
object MathSettingsCalculatorObject
```

## Properties

`BasicMode`

MathSettingsCalculator_BasicModeObject

If present, configures the basic mode of the calculator. Basic mode is always enabled.

`InputModes`

MathSettingsCalculator_InputModesObject

If present, controls global input options of the calculator. If not present, all input modes are enabled.

`MathNotesMode`

MathSettingsCalculator_MathNotesModeObject

If present, configures the Math Notes mode of the calculator. If not present, Math Notes mode is enabled.

`ProgrammerMode`

MathSettingsCalculator_ProgrammerModeObject

If present, configures the programmer mode of the calculator. If not present, programmer mode is enabled.

`ScientificMode`

MathSettingsCalculator_ScientificModeObject

If present, configures the scientific mode of the calculator. If not present, scientific mode is enabled.

## See Also

### Supporting Objects

object MathSettingsCalculator_BasicModeObject

The declaration to configure basic mode in the calculator app.

object MathSettingsCalculator_InputModesObject

The declaration to configure the input modes in the calculator app.

object MathSettingsCalculator_MathNotesModeObject

The declaration to configure Math Notes in the calculator app.

object MathSettingsCalculator_ProgrammerModeObject

The declaration to configure programmer mode in the calculator app.

object MathSettingsCalculator_ScientificModeObject

The declaration to configure scientific mode in the calculator app.

object MathSettingsSystemBehaviorObject

The declaration to configure math behavior at the system level.

