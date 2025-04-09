# Laplacian Pyramid Image Compression

This repository contains the code and notebooks developed as part of the "Technology and Analysis of Image and Video" course assignment. The assignment focuses on the implementation of image compression and progressive transmission techniques using Laplacian pyramids. The work is based on the paper:

**"The Laplacian Pyramid as a Compact Image Code"**  
*Peter J. Burt and Edward H. Adelson, IEEE Transactions on Communications, Vol. COM-31, No. 4, April 1983*

## Overview

In this project, the following tasks have been implemented:
- **Gaussian Pyramid Construction:** Creating a multi-scale representation of an image by iteratively applying low-pass filtering and downsampling.
- **Laplacian Pyramid Construction:** Deriving a Laplacian pyramid by computing the difference between successive levels of the Gaussian pyramid. This step results in a compact representation that emphasizes the image's details.
- **Progressive Transmission:** Demonstrating how the Laplacian pyramid can be used to progressively transmit an image, starting from a coarse version and refining to the original quality.
- **Quantization & Entropy Analysis:** Evaluating the effect of different parameters (such as the generating kernel parameter `a`, pyramid depth, and various bin sizes) on the quality and compression rate. This includes calculating metrics such as entropy and variance to optimize the performance.

Two different quantization schemes are also implemented, where the bin sizes vary per pyramid level:
1. **Example 1:** Larger bin sizes in the lower (detail-rich) levels and smaller bins in the higher (coarser) levels.
2. **Example 2:** Smaller bin sizes in the lower levels and larger bins in the higher levels.
