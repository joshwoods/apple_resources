

- Kernel
-  AppleDSP 

API Collection

# AppleDSP

Perform digital signal processing on data.

## Topics

### Biquadratic Infinite Impulse Response (IIR) Filters

vDSP_biquad2

Applies a single-precision stereo biquadratic IIR filter.

vDSP_biquad2_CreateSetup

Builds a data structure that contains precalculated single-precision data for stereo biquadratic filter functions to use.

IIRChannel

Constants that specify which channels a stereo biquadratic filter operates.

vDSP_biquad2_CopyState

Copies the filter state from one biquadratic filter object to another.

vDSP_biquad2_ResetState

Resets the filter state of a single-precision stereo biquadratic filter object.

vDSP_biquad2_DestroySetup

Destroys a single-precision stereo biquadratic IIR setup object.

### Recursive Filters

vDSP_deq22

Performs two-pole, two-zero recursive filtering on a single-precision vector.

### Conversion Functions

vDSP_vsmfix24

Scales and converts single-precision floating-point values to signed 24-bit integer values.

vDSP_vsmfixu24

Scales and converts single-precision floating-point values to unsigned 24-bit integer values.

vDSP_vfix16

Converts an array of single-precision floating-point values to signed 16-bit integer values, rounding toward zero.

vDSP_vfix32

Converts an array of single-precision floating-point values to signed 32-bit integer values, rounding toward zero.

vDSP_vflt16

Converts an array of signed 16-bit integers to single-precision floating-point values.

vDSP_vflt24

Converts signed 24-bit integer values to single-precision floating-point values.

vDSP_vflt32

Converts an array of signed 32-bit integers to single-precision floating-point values.

vDSP_vfltu24

Converts unsigned 24-bit integer values to single-precision floating-point values.

### Convolution and Correlation Functions

vDSP_conv

Performs either correlation or convolution on two real single-precision vectors.

### Vector Absolute Functions

vDSP_vabs

Calculates the absolute value of each element in the supplied single-precision vector using the specified stride.

### Vector Arithmetic Functions

vDSP_vadd

Adds two single-precision vectors.

vDSP_vma

Adds a single-precision vector to the product of two single-precision vectors.

vDSP_vsub

Subtracts two single-precision vectors.

vDSP_vmul

Multiplies two single-precision vectors.

vDSP_vsmul

Multiplies a single-precision scalar value by a single-precision vector.

vDSP_vdiv

Divides two single-precision vectors.

### Vector Extrema Functions

vDSP_maxmgv

Calculates the maximum magnitude in a single-precision vector.

### Vector Reduction Functions

vDSP_rmsqv

Calculates the root mean square of a single-precision vector.

vDSP_svesq

Calculates the sum of values and the sum of squares in a single-precision vector.

vDSP_svs

Calculates the sum of signed squares in a single-precision vector.

## See Also

### Utilities

Debugging

Debug your kernel extensions using the kernel debugger, assertions, exceptions, backtraces, and logging.

