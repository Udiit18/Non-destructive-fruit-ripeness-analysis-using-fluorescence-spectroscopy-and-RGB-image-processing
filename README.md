# FruitRipeness

## Overview

FruitRipeness is a data analysis project focused on non-destructive
assessment of fruit maturity using fluorescence spectroscopy and RGB
image analysis.

The study analyzes: - Orange (*Citrus reticulata*) - Indian jujube
(*Ziziphus mauritiana*)

Three maturity stages are considered: unripe, mid-ripe, and ripe.

## Objective

The project uses optical measurements and data analysis to distinguish
fruit maturity without damaging the samples.

The analysis includes: - Fluorescence spectral analysis - Spectral
feature extraction - Spectral normalization - Spectral ratio analysis -
RGB image analysis - Color-ratio analysis - Data visualization

## Fluorescence Spectroscopy

Fruit samples were analyzed using visible-light-excited fluorescence
spectroscopy with 405 nm excitation.

Key wavelength regions include: - \~520/545 nm --- carotenoid-related
region - \~684 nm --- chlorophyll a - \~737 nm --- chlorophyll b

The workflow includes processing spectral measurements, averaging
sub-samples, normalization, extracting intensities at selected
wavelengths, calculating spectral ratios, and visualizing changes across
maturity stages.

## Spectral Indicators

### Orange

-   `I684 / I545`
-   `I684 / I737`
-   `(I684 + I737) / I545`

### Indian Jujube

-   `I684 / I520`
-   `I684 / I737`
-   `(I684 + I737) / I520`

These indicators are used to study changes in chlorophyll and
carotenoid-related spectral features during ripening.

## RGB Image Analysis

RGB images were analyzed to obtain color-based indicators of maturity,
including: - RGB feature extraction - R/G ratio - R/B ratio - Color
trend visualization

For orange, additional CIELAB-related features and the Citrus Color
Index (CCI) were analyzed.

## Results

The spectral analysis shows a decrease in chlorophyll-related ratios as
the fruits progress from unripe to ripe stages.

Orange shows the visual transition:

**Green → Yellow → Orange**

Indian jujube shows:

**Green → Yellow-Orange → Orange-Brown**

RGB analysis provides an independent color-based comparison and supports
the trends observed from the fluorescence data.

## Project Structure

``` text
FruitRipeness/
├── Data/
│   ├── Jujube/
│   └── Orange/
├── RGB_Jujube_Results/
├── RGB_Orange_Results/
├── Setup/
├── Spectral_Jujube_Results/
├── Spectral_Orange_Results/
├── MaskCircle.ipynb
├── RGB_Jujube.ipynb
├── RGB_Orange.ipynb
├── Spectral_Jujube.ipynb
├── Spectral_Orange.ipynb
├── Report.pdf
└── SpotSize_on_sample.txt
```

## Technologies

-   Python
-   Jupyter Notebook
-   NumPy
-   Matplotlib
-   SciPy
-   OpenCV
-   scikit-image
-   Fluorescence Spectroscopy
-   RGB Image Analysis
-   Data Visualization

## Key Findings

The project demonstrates how optical data can be used to characterize
fruit maturity through measurable changes in spectral and color
features.

Fluorescence measurements show decreasing chlorophyll-related indicators
with ripening, while RGB analysis provides additional evidence of
corresponding color changes.

## Report

See `Report.pdf` for the detailed methodology, experimental setup,
analysis, results, and conclusions.

## Author

**Udit Chauhan**

M.Tech, IIT Kanpur
