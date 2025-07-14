

- Accelerate
- Fast Fourier transforms
-  Out-of-Place Functions for 1D Real FFT 

API Collection

# Out-of-Place Functions for 1D Real FFT

Perform fast Fourier transforms out of place on 1D real data.

## Overview

The functions in this group use the following operation for a forward real-to-complex transform:

```
N = 1 realp[j*IA];
    h[2*j + 1] = A->imagp[j*IA];
}

// Perform Discrete Fourier Transform.
for (k = 0; k realp[0] and C->imagp[0].
C->realp[0*IC] = Re(H[ 0 ]).
C->imagp[0*IC] = Re(H[N/2]).

// Store regular components:
for (k = 1; k realp[k*IC] = Re(H[k]);
    C->imagp[k*IC] = Im(H[k]);
}

```

The functions in this group use the following operation for an inverse complex-to-real transform:

```
N = 1 realp[0*IA];
h[N/2] = A->imagp[0*IA];
for (j = 1; j realp[j*IA] + i * A->imagp[j*IA];
    h[N-j] = conj(h[j]);
}

// Perform Discrete Fourier Transform.
for (k = 0; k realp[k*IC] = H[2*k+0];
    C->imagp[k*IC] = H[2*k+1];
}

```

The temporary buffer versions perform the same operation but use a temporary buffer for improved performance.

## Topics

### Out-of-Place FFT Functions

vDSP_fft_zrop

Computes a forward or inverse out-of-place, single-precision real FFT.

vDSP_fft_zropD

Computes a forward or inverse out-of-place, double-precision real FFT.

### Out-of-Place FFT Functions with Temporary Buffer

vDSP_fft_zropt

Computes a forward or inverse out-of-place, single-precision real FFT using a temporary buffer.

vDSP_fft_zroptD

Computes a forward or inverse out-of-place, double-precision real FFT using a temporary buffer.

## See Also

### Functions for 1D Real FFT

In-Place Functions for 1D Real FFT

Perform fast Fourier transforms in place on 1D real data.

