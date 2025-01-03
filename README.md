# SESAME BEATS - Cultural Heritage vitreous materials research

CT reconstruction and image processing pipelines for cultural heritage Synchrotron X-ray Computed Tomography (SXCT) scans at beamline [ID10-BEATS](https://www.sesame.org.jo/beamlines/beats) of SESAME.
All pipelines can be found in the [Image processing notebooks](./notebooks) folder.

[![GitHub license](https://img.shields.io/github/license/gianthk/BEATS-CH2024)](https://github.com/gianthk/BEATS-CH2024/blob/master/LICENSE)

- By [Gianluca Iori](https://github.com/gianthk), [Philipp Hans](https://github.com/phlpphns), 2024
- Code licence: MIT
- Narrative licence: CC-BY
- Created on:  05.05.2024
- Last update: 03.01.2025

## Pipelines
| Notebook                    | Description             | Binder URL |
|:----------------------------|:------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------|
| **BEATS_recon_Roman_glass.ipynb**       | Phase-contrast SXCT reconstruction pipeline | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/gianthk/BEATS-CH2024/HEAD?labpath=notebooks%2FBEATS_recon_Roman_glass.ipynb) |
| **BEATS_image_filtering_pipeline.ipynb** | Image filtering facilitating segmentation of large 3D volume | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/gianthk/BEATS-CH2024/HEAD?labpath=notebooks%2FBEATS_image_filtering_pipeline.ipynb) |
| **BEATS_egyptian_blue_pore_size.ipynb** | Plot and visualize results from analysis of porous material | [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/gianthk/BEATS-CH2024/5f2578d3fc41c8ca5f1adbd4553469ffeb56d827?urlpath=lab%2Ftree%2Fnotebooks%2FBEATS_egyptian_blue_pore_size.ipynb) |


## Synchrotron X-ray micro Computed Tomography scans

| Beamline information |                     |
|:---------------------|:--------------------|
| Beamline             | [ID10-BEATS@SESAME](https://www.sesame.org.jo/beamlines/beats) |
| Beamtime             | In-House research   |

- The underlying data for this submission is propertary and subject to embargo according to SESAME's data policy.
- The pipeline for reconstruction of phase-contrast SXCT images can be reproduced using the following open-source dataset from SESAME ID10-BEATS.

| Dataset name                | Description             | DOI        |
|:----------------------------|:------------------------|:-----------|
| `bee_yazeed-20231001T170032.h5` | SXCT scan of a wasp | [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.10075277.svg)](https://doi.org/10.5281/zenodo.10075277) |

### Sample and scan settings

| Sample   | Egyptian blue                            |
|:-----------------------|:-------------------------------|
| Scan name              | egyptian_blue-20240229T135258   |
| Energy                 | 45 keV                         |
| Detector               | Det 2 (Hasselblad system)      |
| Camera                 | PCO.edge 5.5          |
| Voxel size             | 3.1 um                         |
| SDD                    | 300 mm                         |


| Sample   | Roman glass                            |
|:-----------------------|:-------------------------------|
| Scan name              | glass_room-M_stitch-20240222T153555   |
| Energy                 | 20 keV                         |
| Detector               | Det 2 (Hasselblad system)      |
| Camera                 | ORYX FLIR 7.1 MP GigE          |
| Voxel size             | 4.5 um                         |
| SDD                    | 250 mm                         |
| Field of view extension | 360-degree x 3 stitch scans |

## Dependencies

### CT reconstruction
The reconstruction pipeline relies on [`TomoPy`](https://tomopy.readthedocs.io/en/stable/) and [`ASTRA`](https://astra-toolbox.com/). Instructions on how to set up a reconstruction `conda` environment for `TomoPy` can be found [here](https://tomopy.readthedocs.io/en/stable/install.html) and [here](https://tomopy.readthedocs.io/en/stable/devguide.html).

> [!TIP]
> At SESAME BEATS, we installed and built `ASTRA` and `TomoPy` from source in a dedicated `conda` environment. Instructions and a list of dependencies can be found [here](https://github.com/gianthk/alrecon/blob/master/envs/install_alrecon_in_tomopy_dev_env.md).

### 3D image processing

A minimal list of dependencies for 3D image processing in Python can be found [here](envs/image-processing.yml).
