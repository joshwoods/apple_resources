

- Accelerate
- Fast Fourier transforms
-  Out-of-Place Functions for 1D Complex FFT 

API Collection

# Out-of-Place Functions for 1D Complex FFT

Perform fast Fourier transforms out of place on 1D complex data.

## Overview

The functions in this group use the following operation for a complex-to-complex transform:

```
N = 1 realp[j*IA] + i * A->imagp[j*IA];

// Perform Discrete Fourier Transform.
for (k = 0; k realp[k*IC] = Re(H[k]);
    C->imagp[k*IC] = Im(H[k]);
}

```

The temporary buffer versions perform the same operation but use a temporary buffer for improved performance.

## Topics

### Out-of-Place FFT Functions

vDSP_fft_zop

Computes a forward or inverse out-of-place, single-precision complex FFT.

vDSP_fft_zopD

Computes a forward or inverse out-of-place, double-precision complex FFT.

### Out-of-Place FFT Functions with Temporary Buffer

vDSP_fft_zopt

Computes a forward or inverse out-of-place, single-precision complex FFT using a temporary buffer.

vDSP_fft_zoptD

Computes a forward or inverse out-of-place, double-precision complex FFT using a temporary buffer.

### Fixed-Length FFT Functions

vDSP_FFT16_copv

Performs a 16-element FFT on interleaved-complex data.

vDSP_FFT32_copv

Performs a 32-element FFT on interleaved-complex data.

vDSP_FFT16_zopv

Performs a 16-element FFT on split-complex data.

vDSP_FFT32_zopv

Performs a 32-element FFT on split-complex data.

### Radix 3 and Radix 5 FFT Functions

vDSP_fft3_zop

Computes a single-precision out-of-place radix-3 complex FFT, either forward or inverse.

vDSP_fft3_zopD

Computes a double-precision out-of-place radix-3 complex FFT, either forward or inverse.

vDSP_fft5_zop

Computes a single-precision out-of-place radix-5 complex FFT, either forward or inverse.

vDSP_fft5_zopD

Computes a double-precision out-of-place radix-5 complex FFT, either forward or inverse.

## See Also

### Functions for 1D Complex FFT

In-Place Functions for 1D Complex FFT

Perform fast Fourier transforms in place on 1D complex data.

