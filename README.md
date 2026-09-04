# Parametric Curve Parameter Estimation

A Python-based nonlinear curve fitting project that estimates the unknown parameters of a 2D parametric curve from observed `(x, y)` data.

## Problem

The objective is to estimate three unknown parameters:

* **θ (theta)** — rotation angle
* **M** — exponential growth/decay parameter
* **X** — horizontal offset

subject to:

* `0° < θ < 50°`
* `-0.05 < M < 0.05`
* `0 < X < 100`

## Methodology

The project uses:

1. Mathematical transformation of the parametric equations
2. Nonlinear least-squares optimization
3. Bounded parameter constraints
4. Numerical error evaluation
5. Actual vs. predicted curve visualization

Optimization is performed using **SciPy's `least_squares`** algorithm.

## Results

The estimated parameters are:

```text
θ = 30°
M = 0.03
X = 55
```

The fitted curve closely matches the observed data with a very small L1 error.

## Technologies

* Python
* NumPy
* Pandas
* SciPy
* Matplotlib

## Project Structure

```text
├── data/
│   └── xy_data.csv
├── src/
├── results/
├── report/
├── main.py
├── requirements.txt
└── README.md
```

## Run

```bash
pip install -r requirements.txt
python main.py
```

## Author

**Arpita Rajput**
VIT Bhopal University
