<img src="https://www.calgary.ca/water/drinking-water/water-supply/_jcr_content/root/maincontentpar/responsivegrid/grid/column-79640082-b047-4226-99b1-cb3bc0a121330/grid_layout/column-8b00e406-5b45-4bb2-b936-36c9bf332d970/image.img.jpeg/1611679762948/bow-glacier-610px.jpeg" alt="Calgary Water Source" />
# Analysis of Water Quality in Calgary

This is a comprehensive statistical modelling attempt of Calgary's water pH via physico-chemical properties of water. Specifically for watershed surface bodies of water around Calgary (rivers, streams, reservoirs, etc..).

## About the Data 

The data is sourced from <a href="https://data.calgary.ca/Environment/Watershed-Surface-Water-Quality-Data/y8as-bmzj/about_data">Open Source Data of Calgary</a>. 

## Collaborators and Contributors

This was a course group project. Teammates are listed in the PDF report. 

**Main Contributions**
1. Assisted in modelling
2. Evaluation of the model through multi-linear regression modelling assumptions and statistical tests
3. Scientific Review  

## Analysis 

We were able to produce the following model: 

$$
\begin{align}
\widehat{pH} = 
\begin{cases} 
5.974 + 0.04906X_{\text{water temp}} + 4.800 \times 10^{-4}X_{\text{conductivity}} + 1.895 \times 10^{-3}X_{\text{turbidity}} + 0.1982X_{\text{oxygen}} \\
- 1.816 \times 10^{-3}X_{\text{oxygen}}^2 - 7.812 \times 10^{-6}X_{\text{water temp}} X_{\text{conductivity}} - 2.555 \times 10^{-5}X_{\text{water temp}} X_{\text{turbidity}} \\
- 4.983 \times 10^{-4}X_{\text{water temp}} X_{\text{oxygen}} + 1.045 \times 10^{-7}X_{\text{conductivity}} X_{\text{turbidity}} - 3.510 \times 10^{-5}X_{\text{conductivity}} X_{\text{oxygen}} \\
- 1.594 \times 10^{-4}X_{\text{turbidity}} X_{\text{oxygen}} \quad \text{(Fall)} \\\\

6.236 + 0.04906X_{\text{water temp}} + 4.800 \times 10^{-4}X_{\text{conductivity}} + 1.895 \times 10^{-3}X_{\text{turbidity}} + 0.1982X_{\text{oxygen}} \\
- 1.816 \times 10^{-3}X_{\text{oxygen}}^2 - 7.812 \times 10^{-6}X_{\text{water temp}} X_{\text{conductivity}} - 2.555 \times 10^{-5}X_{\text{water temp}} X_{\text{turbidity}} \\
- 4.983 \times 10^{-4}X_{\text{water temp}} X_{\text{oxygen}} + 1.045 \times 10^{-7}X_{\text{conductivity}} X_{\text{turbidity}} - 3.510 \times 10^{-5}X_{\text{conductivity}} X_{\text{oxygen}} \\
- 1.594 \times 10^{-4}X_{\text{turbidity}} X_{\text{oxygen}} + 0.2624 - 8.893 \times 10^{-3}X_{\text{water temp}} \\
+ 6.680 \times 10^{-5}X_{\text{conductivity}} - 6.210 \times 10^{-4}X_{\text{turbidity}} - 1.578 \times 10^{-2}X_{\text{oxygen}} \quad \text{(Spring)} \\\\

6.130 + 0.04906X_{\text{water temp}} + 4.800 \times 10^{-4}X_{\text{conductivity}} + 1.895 \times 10^{-3}X_{\text{turbidity}} + 0.1982X_{\text{oxygen}} \\
- 1.816 \times 10^{-3}X_{\text{oxygen}}^2 - 7.812 \times 10^{-6}X_{\text{water temp}} X_{\text{conductivity}} - 2.555 \times 10^{-5}X_{\text{water temp}} X_{\text{turbidity}} \\
- 4.983 \times 10^{-4}X_{\text{water temp}} X_{\text{oxygen}} + 1.045 \times 10^{-7}X_{\text{conductivity}} X_{\text{turbidity}} - 3.510 \times 10^{-5}X_{\text{conductivity}} X_{\text{oxygen}} \\
- 1.594 \times 10^{-4}X_{\text{turbidity}} X_{\text{oxygen}} + 0.1568 - 3.416 \times 10^{-3}X_{\text{water temp}} \\
+ 6.754 \times 10^{-5}X_{\text{conductivity}} - 4.797 \times 10^{-4}X_{\text{turbidity}} - 2.061 \times 10^{-2}X_{\text{oxygen}} \quad \text{(Summer)} \\\\

5.559 + 0.04906X_{\text{water temp}} + 4.800 \times 10^{-4}X_{\text{conductivity}} + 1.895 \times 10^{-3}X_{\text{turbidity}} + 0.1982X_{\text{oxygen}} \\
- 1.816 \times 10^{-3}X_{\text{oxygen}}^2 - 7.812 \times 10^{-6}X_{\text{water temp}} X_{\text{conductivity}} - 2.555 \times 10^{-5}X_{\text{water temp}} X_{\text{turbidity}} \\
- 4.983 \times 10^{-4}X_{\text{water temp}} X_{\text{oxygen}} + 1.045 \times 10^{-7}X_{\text{conductivity}} X_{\text{turbidity}} - 3.510 \times 10^{-5}X_{\text{conductivity}} X_{\text{oxygen}} \\
- 1.594 \times 10^{-4}X_{\text{turbidity}} X_{\text{oxygen}} - 0.4149 + 2.363 \times 10^{-2}X_{\text{water temp}} \\
- 3.393 \times 10^{-5}X_{\text{conductivity}} - 2.229 \times 10^{-4}X_{\text{turbidity}} + 2.777 \times 10^{-2}X_{\text{oxygen}} \quad \text{(Winter)} \\\\
\end{cases}
$$

The model has an adjusted R-squared 0.5369 with 0.2032 residual standard error. The model explains 53.69% of the variation found in the dependent variable, pH.
