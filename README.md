# Mean-Variance-Standard-Deviation-Calculator

This project contains a Python function, `calculate()`, which performs statistical analysis on a 3x3 matrix using NumPy. The function computes key metrics, including the mean, variance, standard deviation, maximum, minimum, and sum along both axes and for the flattened matrix.

## Features

The `calculate()` function:
- Takes a list of 9 numerical values as input.
- Converts the list into a 3x3 NumPy array.
- Calculates the following statistics:
  - **Mean**
  - **Variance**
  - **Standard Deviation**
  - **Maximum**
  - **Minimum**
  - **Sum**
- Returns the results in a structured dictionary format.

### Output Format

The returned dictionary includes results for each statistic along:
- Axis 0 (columns)
- Axis 1 (rows)
- The flattened matrix

Example output for `calculate([0,1,2,3,4,5,6,7,8])`:
```python
{
  'mean': [[3.0, 4.0, 5.0], [1.0, 4.0, 7.0], 4.0],
  'variance': [[6.0, 6.0, 6.0], [0.6666666666666666, 0.6666666666666666, 0.6666666666666666], 6.666666666666667],
  'standard deviation': [[2.449489742783178, 2.449489742783178, 2.449489742783178], [0.816496580927726, 0.816496580927726, 0.816496580927726], 2.581988897471611],
  'max': [[6, 7, 8], [2, 5, 8], 8],
  'min': [[0, 1, 2], [0, 3, 6], 0],
  'sum': [[9, 12, 15], [3, 12, 21], 36]
}
```

## Error Handling

- If the input list contains fewer than 9 elements, the function raises a `ValueError` with the message:
  ```
  List must contain nine numbers.
  ```

## Development

- **Implementation:** Write the code in `mean_var_std.py`.
- **Testing:** Use `main.py` for development and manual testing.
  - Run the script with:
    ```bash
    python3 main.py
    ```

## Testing

Unit tests for the function are provided in `test_module.py`. These tests are also imported into `main.py` for convenience. To run all tests, execute:
```bash
python3 main.py
```
