title: Command Line Interface
---

ITK/VTK Image Viewer can be used as a command line tool for opening and visualizing your local data file.

## Installation

First, [install Node.js](https://nodejs.org/en/download/) if not already
installed; after installed, `node` and `npm` should be in your `PATH`.

```sh
$ npm install itk-vtk-viewer -g
```

The command line will install globally the application which should enable a new command line:

```sh
$ itk-vtk-viewer

  Usage: itk-vtk-viewer [options] ] [inputFile]

    Options:

    -V, --version      output the version number
    -p, --port [3000]  Start web server with given port (default: 3000)
    -s, --server-only  Do not open the web browser

    -h, --help         output usage information
```

## Usage

Listed above are the various options available, but below are commonly used commands:


### Quick start

To visualize an image, in the path to the file to visualize. By default, a new
tab will open in you browser with your visualization.

```sh
$ itk-vtk-viewer ./MRHead.nrrd

itk-vtk-viewer
  => Serving .

       http://10.10.10.10:3000/?fileToLoad=/data/MRHead.nrrd
```

### Drag and drop viewer

Instead of specifying files via the command line, drag and drop, click on the
viewer page, or press the *Enter* key to select a file after starting without
positional arguments:

```sh
$ itk-vtk-viewer
```

![ItkVtkViewer](./viewer.jpg)
