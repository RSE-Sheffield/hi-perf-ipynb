#  Notes that may be useful later

## mkl service functions

`mkl.get_cpu_clocks()` -> `int`
    Return the CPU clocks as an integer.
`mkl.get_cpu_frequency()` -> `float`
    Return CPU frequency in GHz as a float.
`mkl.get_max_threads()` -> `int`
    Return the number of threads Intel MKL is targeting for parallelism.
`mkl.get_version_string()` -> `str`
    Return the MKL library version information as a string.
`mkl.mem_stat()` -> (`int`, `int`)
    Returns a tuple (bytes, count) containing memory usage statistics of the MKL allocator - number of bytes allocated (bytes). - number of allocated blocks (count).
`mkl.set_num_threads(n)`
    Set the number of threads MKL should use. This is only a hint, and no guaranteed is made this number of threads will actually be used. This function takes precedence over the environment variable `MKL_NUM_THREADS`. 
