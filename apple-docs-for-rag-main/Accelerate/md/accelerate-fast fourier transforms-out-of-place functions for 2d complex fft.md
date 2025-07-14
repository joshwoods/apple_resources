

- Accelerate
- Fast Fourier transforms
-  Out-of-Place Functions for 2D Complex FFT 

API Collection

# Out-of-Place Functions for 2D Complex FFT

Perform fast Fourier transforms out of place on 2D complex data.

## Overview

The functions in this group use the following operation for a complex-to-complex transform:

```

N0 = 1 realp[j1*IA1 + j0*IA0]
          + i * A->imagp[j1*IA1 + j0*IA0];

// Perform Discrete Fourier Transform.
for (k1 = 0; k1 realp[k1*IC1 + k0*IC0] = Re(H[k1][k0]);
    C->imagp[k1*IC1 + k0*IC0] = Im(H[k1][k0]);
}

```

The temporary buffer versions perform the same operation but use a temporary buffer for improved performance.

## Topics

### Out-of-Place FFT Functions

vDSP_fft2d_zop

Computes a 2D forward or inverse out-of-place, single-precision complex FFT.

vDSP_fft2d_zopD

Computes a 2D forward or inverse out-of-place, double-precision complex FFT.

### Out-of-Place FFT Functions with Temporary Buffer

vDSP_fft2d_zopt

Computes a 2D forward or inverse out-of-place, single-precision complex FFT using a temporary buffer.

vDSP_fft2d_zoptD

Computes a 2D forward or inverse out-of-place, double-precision complex FFT using a temporary buffer.

## See Also

### Functions for 2D Complex FFT

In-Place Functions for 2D Complex FFT

Perform fast Fourier transforms in place on 2D complex data.

