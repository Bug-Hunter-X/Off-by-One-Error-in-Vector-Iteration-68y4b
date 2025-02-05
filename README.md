# Off-by-One Error in C++ Vector Iteration

This repository demonstrates a common off-by-one error in C++ when iterating over a `std::vector`.  The error occurs because the loop condition `i <= vec.size()` allows access to an element beyond the valid range of the vector.

**Bug:** The provided code attempts to access `vec[vec.size()]`, which is one element past the end of the vector. This leads to undefined behavior.

**Solution:** Correct the loop condition to `i < vec.size()` to ensure that the loop only iterates over valid indices.
