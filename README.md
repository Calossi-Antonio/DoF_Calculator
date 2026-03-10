# Functional Depth of Focus (DoF) Calculator

This repository hosts the official computational tool for the objective quantification of **Functional Depth of Focus (DoF)** from discrete defocus-acuity data, as presented in our study published in the *Journal of Cataract & Refractive Surgery (JCRS)*.

## Overview

Quantifying Depth of Focus is often prone to subjective variability due to the manual inspection of defocus curves. This Excel-based tool standardizes the process using a **linear interpolation algorithm**, providing a reproducible and mathematically rigorous method to identify threshold crossings.

## Key Features

* **Precise Linear Interpolation:** Automatically calculates near ($N$) and far ($P$) dioptric intersections at any user-defined $logMAR$ threshold.
* **Dual-Threshold Reporting:** Optimized for reporting both "High-Acuity DoF" ($0.1$ $logMAR$) and "Functional DoF" ($0.2$ $logMAR$).
* **Automated Continuity Check (Dip-Check):** Detects non-monotonic curves and flags "discontinuous ranges" to prevent inflated DoF values in multifocal or bifocal lens designs.
* **Range Validity Safeguards:** Identifies and flags intersections that fall outside the tested dioptric boundaries, ensuring conservative and honest reporting.
* **Standardized Data Entry:** A clean, matrix-style interface for clinical data (Patient ID, Eye, and defocus steps).

## How to Use

1.  **Download:** Download the `Functional_DoF_Calculator.xlsx` file from this repository.
2.  **Set Threshold:** Enter your target $logMAR$ threshold in cell **B1** (e.g., $0.2$).
3.  **Input Data:** Replace the example clinical data in the white cells (Columns **C** to **N**) with your own measurements.
4.  **Analyze:** The results for Near Limit, Far Limit, and Total DoF will update automatically in columns **W**, **X**, and **Y**.
5.  **Review Flags:** Check columns **AD** and **AE** for any automated warnings regarding range limits or curve continuity.

## Requirements

* Microsoft Excel 2016 or later (compatible with Windows and macOS).
* No additional plugins or VBA macros are required (all formulas are natively implemented for transparency).

## Citation

If you use this calculator or the underlying algorithm in your research, please cite our original work:

> **Calossi A. et al** *A standardized method for Functional Depth of Focus calculation* **J Cataract Refract Surg. 2026.** [Link al DOI se disponibile]

## License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details. This means you are free to use, modify, and distribute the tool, provided that credit is given to the original authors.

## Contact

For questions, feedback, or to report issues, please contact:
**Antonio Calossi** - antonio.calossi@gmail.com
