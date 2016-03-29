#### utilities
| | |
| :--- | :--- |
| `lsi` | ("list images") tabulate image files along with output from `fslinfo` and `fslstats` |
| `mm2label` | get labels from FSL atlases and Talairach Daemon<sup>1</sup> |
| `fslmathses`<sup>2</sup> | `fslmaths` + a few operators (e.g., correlation) + functionality from `fslstats` + ability to write nested commands |
| `findMNI` | fetches path of various standard brains |
| `intsub` | do intensity substitution (e.g., `data[data==x] = y`)|
| `lst2nii` | specify an image in a plain text list of voxels + intensities |

<sup>1</sup> if TD is installed on your system... probably requires adjustment

<sup>2</sup> I've come across some suspicious behavior from this (e.g., correlation coeffs >1 (rounding errors?)), use with caution!

#### images, statmaps
|  | |
| :--- | :--- |
| `imagethresher` | voxelwise, clusterwise thresholding of stat maps in various ways (binarized, indexed, pruned, ...) |
| `clustertable` | produce a table of clusters in an image (extends `cluster`) |
| `mkmask` | make spherical, cubic masks in MNI space |
| `mkatlasmask` | make masks based on atlases available in FSL |

#### viewing images (FSLview wrappers)
| | |
| :--- | :--- |
| `zview` | primarily intended for zstat overlays, but will attempt to detect several other sorts of images (binarized, indexed, etc) |
| `fslviewdiffs` | calculate the difference between statmaps (several method options) and open in FSLview |
| `prunethresh` | for use with `-prune` option output of `imagethresher` |
| `tview` | for use with t stat map outputs of SPM analyses |

#### FEAT tools
| | |
| :--- | :--- |
| `fsfinfo` | Print properties of FEAT designs. For higher levels will retrieve properties of inputs/lower levels |

#### coordinate conversion
| | |
| :--- | :--- |
| `mm2vox`, `vox2mm` | convert MNI millimeter cooridinates to MNI voxel coordinates and vice versa (simplifies `img2stdcoord`, etc) |
| `mni2tal` | convert from MNI to Talairach coordinates (mm) |




