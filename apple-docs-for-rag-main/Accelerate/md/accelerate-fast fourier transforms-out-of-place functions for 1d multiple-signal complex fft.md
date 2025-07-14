

- Accelerate
- Fast Fourier transforms
-  Out-of-Place Functions for 1D Multiple-Signal Complex FFT 

API Collection

# Out-of-Place Functions for 1D Multiple-Signal Complex FFT

Perform fast Fourier transforms out of place on multiple-signal 1D complex data.

## Overview

The functions in this group use the following operation for a complex-to-complex transform:

```
N = 1 realp[m*IMA + j*IA] + i * A->imagp[m*IMA + j*IA];

    // Perform Discrete Fourier Transform.
    for (k = 0; k realp[m*IM + k*IC] = Re(H[k]);
        C->imagp[m*IM + k*IC] = Im(H[k]);
    }
}

```

The temporary buffer versions perform the same operation but use a temporary buffer for improved performance.

## Topics

### Out-of-Place FFT Functions

vDSP_fftm_zop

Computes a forward or inverse out-of-place, single-precision complex FFT on multiple signals.

vDSP_fftm_zopD

Computes a forward or inverse out-of-place, double-precision complex FFT on multiple signals.

### Out-of-Place FFT Functions with Temporary Buffer

vDSP_fftm_zopt

Computes a forward or inverse out-of-place, single-precision complex FFT on multiple signals using a temporary buffer.

vDSP_fftm_zoptD

Computes a forward or inverse out-of-place, double-precision complex FFT on multiple signals using a temporary buffer.

## See Also

### Functions for 1D Multiple-Signal Complex FFT

In-Place Functions for 1D Multiple-Signal Complex FFT

Perform fast Fourier transforms in place on multiple-signal 1D complex data.

