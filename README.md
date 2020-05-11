Gimel Studio
============

Gimel Studio is a **non-destructive, realtime image graphics editing software program** for Windows and Linux.

!["Gimel Studio"](/screenshots/gimel-studio-photo-editing.JPG?raw=true "Gimel Studio")

# Introduction

Gimel Studio has a node-based workflow for realtime compositing, manipulating, generating and adding effects to images -complete with a registry of 10+ nodes (currently) and an API allowing users to script their own custom nodes.

It provides basic image editing features such as rotate, resize and blur effects, as well as more advanced editing capabilities such as generating normal maps for use in 3D from images.

*Still in BETA stage, but can be considered stable enough for light production work.*

**Your are welcome to help develop Gimel Studio**

See the [ROADMAP.txt](ROADMAP.txt) for a general idea of the possible future goals of the development of Gimel Studio - or, if you are interested in helping out wherever, look throught the code for the ``TODOS``. :)

# Features

**Highlights**
  
  * Written in pure Python with minimal dependancies
  * Support for opening and saving your nodegraph as a GIMEL-STUDIO-PROJECT
  * 10+ nodes (currently) with a wide range of functionality 
  * Rearrangable and resizable panels for the main UI
  * Drag 'n drop nodes from the Node Registry
  * Node-based workflow (similar to Blender 3D)
  * JPEG, PNG, BMP file types support
  * API for scripting custom nodes
  * Zoomable Image Viewport for viewing renders in real-time

**Tidbits**

  * Auto-renders as the Node Graph is edited
  * Toggle-able thumbnails on nodes showing the steps of the rendered image


# Releases

**Latest release:** Gimel Studio 0.1.8 was released "May" 2020.

Head to the <a href="https://correctsyntax.com/projects/gimel-studio/">Gimel Studio homepage</a> to download the latest release or <a href="https://github.com/Correct-Syntax/Gimel-Studio/releases">click here</a> to see past releases on Github.

# Documentation

You can find the latest documentation at the <a href="https://correctsyntax.com/projects/gimel-studio/">Gimel Studio homepage</a> or build it yourself following the steps in the section *Building the documentation from source* below.

Documentation for past Gimel Studio releases can be <a href="https://github.com/Correct-Syntax/Gimel-Studio/releases">here</a>.

# Installing from source

Gimel Studio is currently written in pure Python, so there shouldn't be any need to compile anything except for the dependancies (in some cases).

This assumes you have **Python 3.6 or higher** installed on your system and you are in the **root directory** of Gimel Studio.

1. First download the tar.gz source archive file from <a href="https://github.com/Correct-Syntax/Gimel-Studio/releases">here.</a> 

  * Extract the archive into an empty folder
  * Get <a href="https://pipenv.pypa.io/en/latest/">pipenv</a>
  * Install the dependencies with ``pipenv install`` 

    This will install the core dependancies for Gimel Studio.

2. Run  ``pipenv shell`` and you should be able to now run 
   ``python "/src/Gimel Studio.py"`` or ``python3 "/src/Gimel Studio.py"`` depending on your setup to launch Gimel Studio.

3. If you want to build Gimel Studio as an .exe for Windows or build an executable for Linux, you will also need the PyInstaller package.

  * Install development dependancies with ``pipenv install --dev``
  * Now run ``./make`` in your Linux Terminal or ``Make.bat`` in your Windows CMD. 

  This should start building Gimel Studio with the appropriate settings for Pyinstaller, and you should find the executable in the ``dist`` folder.


# Build the development version

The development version of Gimel Studio may be unstable and/or have new dependencies. If you fail to install the development version, please file a bug in Issues -tab.

1. Install Git in your system

2. Use Git to download Gimel Studio into a folder of your choosing by using the git clone command in a terminal or CMD:
  * Clone the repo with ``git clone https://github.com/Correct-Syntax/Gimel-Studio.git``

3. Follow the steps listed in the *Installing from source* section above.


# Building the documentation from source

The Gimel Studio docs use the Sphinx package.
  
  * Get <a href="https://pipenv.pypa.io/en/latest/">pipenv</a>
  * Install development dependancies with ``pipenv install --dev``
  * ``pipenv shell``
  * ``cd docs``
  * Now run ``make html`` to build the docs.

You will find the HTML docs in the ``build`` folder.


# License

Gimel Studio is licensed under the Apache License, Version 2.0. See the LICENSE and NOTICE files for full copyright and license information.
