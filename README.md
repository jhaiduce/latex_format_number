# latex_format_number

latex_format_number formats numbers using LaTeX equation syntax

## Getting started

### Prerequisites

- python 2.7 or 3.x

### Installing

```shell
python setup.py install
```

### Example

```python
from latex_format_number import latex_format_number
latex_format_number(1,0.1)    # Returns '1.0\pm0.1'
latex_format_number(1234,100) # Returns '1200\pm100'
latex_format_number(1e5,10)   # Returns '1.000\times10^{4}\pm10'
latex_format_number(0,(2,1))  # Returns '0[+2,-1]'
latex_format_number(0.016,0.01,
	overline=True,
	extra_digits=1)       # Returns '0.0\\overline{1}6\\pm0.01'
```