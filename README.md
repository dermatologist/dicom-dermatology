# DICOM 4 Dermatology

## About
This is a meta-repository of dicoderma (a Java library) and dit4ij (an ImageJ plugin). [Read this paper]() for more information.

### [dicoderma](https://github.com/dermatologist/dicoderma)
Dermatology never really embraced DICOM for image management. Dicoderma is an attempt to narrow the rift by freeing dermatologists from the overhead of DICOM compliant infrastructure but gives some of the advantages like storing patient metadata with images. Dicoderma facilitates this by mapping DICOM tags to EXIF USER_CONTENT. You can also convert JPEG to DCM.  [More...](https://github.com/dermatologist/dicoderma)

### [dit4ij](https://github.com/dermatologist/dit4ij)
ImageJ (and its batteries-included version, [Fiji](https://fiji.sc/)) is a popular biomedical imaging software with a modular, extensible architecture. ImageJ can be downloaded from the NIH website [here](https://imagej.nih.gov/ij/download.html). DIT4IJ is an ImageJ plugin that adds DICOM related function for clinical images in Dermatology. It adds certain DICOM tags as a JSON formatted string to the EXIF header that can be used for searching. It also supports converting general images to DICOM (.dcm) resources that can be used with the DICOM supported systems such as PACS. [More](https://github.com/dermatologist/dit4ij)

### Requirements
* java8
* maven
* ImageJ

### How to build
**We do not provide pre-built binaries**
```
git clone --recurse-submodules https://github.com/dermatologist/dicom-dermatology.git
cd dicoderma
mvn -Dmaven.test.skip=true clean install
cd ../dit4ij
mvn -Dmaven.test.skip=true clean package
```
* This generates the plugin file dit4ij-VERSION-.jar in the target folder.
* Install the plugin in ImageJ as described [here](https://imagej.net/Installing_3rd_party_plugins).

### [Demonstration video]()

### Contributing
Please submit pull requests in the submodules.

### Citation
Please cite this work as below. [Read paper]()

```
More
```
