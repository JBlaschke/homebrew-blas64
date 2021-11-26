# Homebrew-BLAS64

`openblas64`: A formula for a 64-bit version of OpenBLAS. In order to avoid
conflicts with existing installations of BLAS (which might rely on the 32-bit
interface), we add the `64_` sufftix. This formula was built using:
`make SYMBOLSUFFIX=64_ INTERFACE64=1 BINARY=64 ...`

This tap also includes formulae that use this 64-bit version of openBLAS:
1. `julia64`