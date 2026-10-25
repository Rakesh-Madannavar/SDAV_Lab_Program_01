# Discrete-Probability-Distributions-AIML-Lab

# Discrete Probability Distributions – AIML Lab

An interactive, single-page web app for exploring discrete probability distributions. It was built as **SDAV Lab Program 01** for the AIML Laboratory.

🔗 **Live demo:** https://rakesh-madannavar.github.io/SDAV_Lab_Program_01/

---

## Overview

Pick a distribution, enter parameters, and see probabilities, statistics and charts update instantly. Everything runs in the browser, with no installation, backend or external libraries.

## Modules

| Module | What it calculates |
|--------|--------------------|
| **Binomial** | Probability of exactly *k* successes in *n* independent trials |
| **Poisson** | Probability of a number of occurrences of an event in a fixed interval |
| **Geometric** | Probability that the first success occurs on a particular trial |

## Features

- **Live calculation:** results refresh as you type
- **Input validation:** clear error message for invalid values (e.g. `n` must be a positive integer, `0 ≤ p ≤ 1`, `0 ≤ k ≤ n`)
- **Probability Mass Function (PMF):** `P(X = k)` shown as a decimal and a percentage
- **Cumulative Distribution Function (CDF):** `P(X ≤ k)` and `P(X > k)`
- **Interactive PMF bar chart:** hover over a bar to see the exact `X` and `P(X)`, with a dashed line marking the mean
- **Summary statistics:** mean, variance, standard deviation, second moment `E[X²]` and skewness
- **Responsive UI:** works on desktop and mobile, with automatic light and dark mode

## Formulas (Binomial module)

```
PMF:       P(X = k) = C(n, k) · p^k · (1 − p)^(n − k)
CDF:       P(X ≤ k) = Σ P(X = i), for i = 0 to k
Mean:      μ  = n · p
Variance:  σ² = n · p · (1 − p)
Skewness:  (1 − 2p) / √(n · p · (1 − p))
E[X²]:     Var(X) + μ²
```

## Tech Stack

- HTML5
- CSS3 (CSS variables, Grid, Flexbox, `light-dark()` theming)
- Vanilla JavaScript (no frameworks or dependencies)

## Project Structure

```
SDAV_Lab_Program_01/
├── index.html    # Complete application (markup, styles and logic)
└── README.md
```

## Getting Started

### Run locally

```bash
# 1. Clone the repository
git clone https://github.com/Rakesh-Madannavar/SDAV_Lab_Program_01.git

# 2. Open the project folder
cd SDAV_Lab_Program_01

# 3. Open index.html in any modern browser
```

No build step or server is required.

## Usage

1. Open the app and choose **Binomial**, **Poisson** or **Geometric** from the top navigation (or click a card on the home page).
2. Enter the parameters for the distribution.
3. Read the probability, CDF, statistics and PMF chart, which all update automatically.

## Author

**Rakesh Madannavar**
GitHub: [@Rakesh-Madannavar](https://github.com/Rakesh-Madannavar)
