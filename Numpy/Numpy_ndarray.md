## Numpy ndarray

### Array Object

ndarray is N-dimensional array object.

### Array Creation

| Function            | Description                                                  |
| ------------------- | ------------------------------------------------------------ |
| `array`             | Convert input data (list, tuple, array, or other sequence type) to an ndarray either by inferring a dtype or explicitly specifying a dtype. Copies the input data by default. |
| `asarray`           | Convert input to ndarray, but do not copy if the input is already an ndarray |
| `arange`            | Like the built-in `range` but returns an ndarray instead of a list. |
| `ones, ones_like`   | Produce an array of all 1’s with the given shape and dtype. `ones_like` takes another array and produces a ones array of the same shape and dtype. |
| `zeros, zeros_like` | Like `ones` and  `ones_like` but producing arrays of 0’s instead |
| `empty, empty_like` | Create new arrays by allocating new memory, but do not populate with any values like `ones` and `zeros` |
| `eye, identity`     | Create a square N x N identity matrix (1’s on the diagonal and 0’s elsewhere) |