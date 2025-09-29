# Stage

Stage is a MATLAB-based visual stimulus system for vision research. It provides a toolbox for writing visual stimulus routines.
This fork is from the original Stage-VSS repository, with all submodules forked as well (other than docs). The purpose of this
fork is to add linux and (eventually) Apple silicon compatibility.

## Clone

`git clone https://github.com/drezeanu/stage.git --recursive`

**Note:** You must use the `--recursive` option to recursively clone all submodules.

## Build

Matlab functions in the root directory are used to build the project. The scripts are named according to the build phase they execute. The phases include:

- `test`: run tests using the Matlab unit test framework
- `package`: package the project into a .mltbx file
- `install`: install the packaged product into Matlab

Similar to the [Maven Build Lifecycle](https://maven.apache.org/guides/introduction/introduction-to-the-lifecycle.html), each phase will execute all phases before it (i.e. running `install` will execute `test`, `package`, `install`). In addition there is a `site` script to generate the project's documentation from the [docs](https://github.com/Stage-VSS/stage-docs) repo.

## Directory Structure

The project directory structure generally follows the [Maven Standard Directory Layout](https://maven.apache.org/guides/introduction/introduction-to-the-standard-directory-layout.html).

## License

Licensed under the [MIT License](https://opensource.org/licenses/MIT), which is an [open source license](https://opensource.org/docs/osd).
