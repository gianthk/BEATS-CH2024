# BEATS - Cultural Heritage 2024

Repository of the image processing software for cultural heritage SXCT scans at SESAME BEATS.

Image processing steps are described in the [Image processing notebooks](./notebooks) folder.

[![GitHub license](https://img.shields.io/github/license/gianthk/BEATS-CH2024)](https://github.com/gianthk/BEATS-CH2024/blob/master/LICENSE)

- By [Gianluca Iori](https://github.com/gianthk), [Philipp Hans](https://github.com/phlpphns), 2024
- Code licence: MIT
- Narrative licence: CC-BY
- Created on:  05.05.2024
- Last update: 05.05.2024

**Synchrotron microCT scan information:**

| Beamline information |                     |
|:---------------------|:--------------------|
| Beamline             | ID10-BEATS @ SESAME |
| Beamtime             | In-House research   |

| Egyptian blue          |                                                     |
|:-----------------------|:----------------------------------------------------|
| Scan name              |                                                     |
| Energy                 | xx keV                                              |
| Detector               | Det 3 (mono microscope)                             |
| Camera                 | PCO.edge 5.5                                        |
| Voxel size             | x.x um                                              |
| SDD                    | xx mm                                               |
| Preliminary operations | ROI crop; 8-bit convert                             |
|                        | k-means segmentation                                |
|                        | isolate large pores                                 |
|                        | calculate pore Mas. Feret diameter                  |
|                        | calculate local thickness map of small pore network |


---
## Acknowledgements

---
Beamtime files (restricted access):
- [Beamtime log]()
- [Beamtime master file]()
