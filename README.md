| utilities | |
| :--- | :--- | :--- |
| `lsi` | ("list images") tabulate images along with output from `fslinfo` and `fslstats` |
| `mm2label` | get labels from FSL atlases and Talairach Daemon<sup>1</sup> |
| `mm2vox`, `vox2mm` | convert MNI millimeter cooridinates to MNI voxel coordinates and vice versa (simplifies `img2stdcoord`, etc) |
| `mni2tal` | convert from MNI to Talairach coordinates (mm) |
| `fslmathses`<sup>2</sup> | `fslmaths` + a few operators (e.g., correlation) + functionality from `fslstats` + ability to write nested commands |
| `findMNI` | fetches path of various standard brains |

<sup>1</sup> if TD is installed on your system... probably requires adjustment

<sup>2</sup> I've come across some suspicious behavior from this (e.g., correlation coeffs >1 (rounding errors?)), use with caution!


| FEAT tools | |
| :--- | :--- |
| `fsfinfo` | Print properties of FEAT designs. For higher levels will retrieve properties of inputs/lower levels |

