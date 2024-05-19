# BEATS - Cultural Heritage 2024

Repository of the image processing software for cultural heritage SXCT scans at SESAME BEATS.

Image processing steps are described in the [Image processing notebooks](./notebooks) folder.

[![GitHub license](https://img.shields.io/github/license/gianthk/BEATS-CH2024)](https://github.com/gianthk/BEATS-CH2024/blob/master/LICENSE)

- By [Gianluca Iori](https://github.com/gianthk), [Philipp Hans](https://github.com/phlpphns), 2024
- Code licence: MIT
- Narrative licence: CC-BY
- Created on:  05.05.2024
- Last update: 19.05.2024

**Synchrotron microCT scan information:**

| Beamline information |                     |
|:---------------------|:--------------------|
| Beamline             | ID10-BEATS @ SESAME |
| Beamtime             | In-House research   |

| Egyptian blue          |                                                     |
|:-----------------------|:----------------------------------------------------|
| Scan name              |                                                     |
| Energy                 | 45 keV                                              |
| Detector               | Det 2 (Hasselblad system)                           |
| Camera                 | PCO.edge 5.5                                        |
| Voxel size             | 6.5 um                                              |
| SDD                    | 300 mm                                              |
| Preliminary operations | ROI crop; 8-bit convert                             |
|                        | k-means segmentation                                |
|                        | isolate large pores                                 |
|                        | calculate pore Mas. Feret diameter                  |
|                        | calculate local thickness map of small pore network |

| Byzantine glass        |                                |
|:-----------------------|:-------------------------------|
| Scan name              |                                |
| Energy                 | 20 keV                         |
| Detector               | Det 2 (Hasselblad system)      |
| Camera                 | ORYX FLIR 7.1 MP GigE          |
| Voxel size             | 4.5 um                         |
| SDD                    | 250 mm                         |
| Preliminary operations | 8-bit convert; stack stitching |


---
## Acknowledgements

---
Beamtime files (restricted access):
- [Beamtime log]()
- [Beamtime master file]()
