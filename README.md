# American Basket Option Pricing with Finite Elements

## Overview

This project implements a **FreeFEM++** solution for pricing **American basket options** using **finite element methods**. Developed as part of the **Applied Numerical Finance** course at **Bocconi University** under the supervision of **Professor Battauz**, this model focuses on pricing American options on the maximum of two assets and compares them with their European counterparts. The core solution involves solving partial differential equations (PDEs) using finite element methods (FEM).

## Key Features

* **American Basket Option Pricing:** Computes the price of an American option on the maximum of two assets
* **Early Exercise Premium:** Calculates the premium associated with the early exercise feature by comparing the American option price with its European equivalent
* **Finite Element Method (FEM):** Leverages the power and flexibility of FreeFEM++, a dedicated PDE solver using FEM, to address the pricing problem
* **Adaptive Mesh Refinement:** Employs adaptive mesh refinement to enhance computational efficiency and accuracy, particularly in critical regions such as the exercise boundary

## Prerequisites

* **FreeFEM++:** Download and install the latest version of FreeFEM++ from the [official website](https://doc.freefem.org/introduction/download.html)

## Installation

1. **Install FreeFEM++:** Follow the instructions on the FreeFEM++ website to install the software for your operating system.

2. **Clone the Repository:** Clone this repository to your local machine using the following command:
   ```bash
   git clone https://github.com/acs-coder/american-basket-options-freefem.git
   ```

3. **Navigate to Project Directory:**
   ```bash
   cd american-basket-options-freefem
   ```

4. **Execute FreeFEM++ Script:** Run the main FreeFEM++ script (e.g., `VIA-american_r2.edp`) using:
   ```bash
   FreeFem++ VIA-american_r2.edp 
   ```

## Usage

The FreeFEM++ script defines various financial parameters, including volatility, risk-free interest rate, and strike price. Modify these input parameters within the script to explore different scenarios:

* `T`: Time to maturity (in years)
* `sigmax`: Volatility of the first asset
* `sigmay`: Volatility of the second asset
* `rho`: Correlation between the two assets
* `r`: Risk-free interest rate
* `K`: Strike price
* `dt`: Time step for numerical solution

## Results

The script produces the computed American basket option price. FreeFEM++ also generates visualizations of the solution. The early exercise premium is calculated by comparing American and European option prices. Adaptive mesh refinement ensures higher accuracy in critical regions, such as near the strike price.

## Technical Documentation

For detailed information about the mathematical formulation, numerical methods, and implementation details, please refer to the [Technical Documentation](docs/technical.md).

## Performance Analysis

Performance benchmarks and accuracy comparisons with other numerical methods can be found in the [Performance Analysis](docs/performance.md) document.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## Acknowledgments

* Professor Battauz for guidance and support during the Applied Numerical Finance course at Bocconi University
* The FreeFEM++ development team for providing this powerful and versatile PDE solver
* Contributors and researchers in the field of computational finance who have laid the groundwork for this implementation

## Contact Information

* **Author:** [Your Name]
* **Email:** [your.email@example.com]
* **LinkedIn:** [Your LinkedIn Profile]
* **Project Link:** [https://github.com/yourusername/american-basket-options-freefem](https://github.com/yourusername/american-basket-options-freefem)

## Citation

If you use this code in your research, please cite:
```bibtex
@misc{american-basket-options-freefem,
  author = {[Your Name]},
  title = {American Basket Option Pricing with Finite Elements},
  year = {2024},
  publisher = {GitHub},
  journal = {GitHub repository},
  url = {https://github.com/yourusername/american-basket-options-freefem}
}
```
