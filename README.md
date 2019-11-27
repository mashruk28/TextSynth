Multi File Format Text Extraction and Text-to-Speech Synthesis
======

<img align="left" width="256" src="https://c7.uihere.com/files/429/478/521/watson-ibm-speech-synthesis-text-computer-software-ibm.jpg"/>

This pre-alpha version of the project is a minimalist implementation of extraction of texts from different file formats such as .txt, .pdf, .png, .jgp (more to be included) and synthesizing texts from the extracted text.

The idea is to provide user accessibility of consumption of textual data from merely visual text to audio text. This enables people with visual acuity or learning disability to understand textual data in a different format that enables them to learn more effectively.

Only three modules (TXT to text, PDF to text and IMG to text) exist as of now in this package. The GUI is made up of Kivy and its sister concern project KivyMD (licensed under MIT).


Installation
============

#### Dependencies:

* [Kivy](https://github.com/kivy/kivy) >= 1.11.1 ([Installation](https://kivy.org/#download))
* [PIL](https://github.com/python-pillow/Pillow) ([Installation](https://pillow.readthedocs.io/en/stable/installation.html#basic-installation))
* [Python 3.6+](https://www.python.org/) *(Python 2 not supported)*

#### How to install

You can install latest release version of KivyMD from [PyPI](https://pypi.org/project/kivymd):
```bash
python3 -m pip install kivymd
```
If you want to install development version from [master](https://github.com/HeaTTheatR/KivyMD/tree/master/) branch, you should specify git HTTPS address:
```bash
# Master branch:
python3 -m pip install git+https://github.com/HeaTTheatR/KivyMD.git
# Specific branch:
python3 -m pip install git+https://github.com/HeaTTheatR/KivyMD.git@stable
# Specific tag:
python3 -m pip install git+https://github.com/HeaTTheatR/KivyMD.git@0.100.2
# Specific commit:
python3 -m pip install git+https://github.com/HeaTTheatR/KivyMD.git@f80d9c8b812d54a724db7eda30c4211d0ba764c2

# If you already has installed KivyMD
python3 -m pip install --force-reinstall git+https://github.com/HeaTTheatR/KivyMD.git
```
Also you can install manually from sources. Just clone the project and run the setup.py script:
```bash
python3 ./setup.py install
```

#### Notes

* The app is tested exclusively on Linux OS with both KivyMD and Kivy libraries installed via 'pip' commands.
* Both Kivy and KivyMD libraries must be installed properly on the environment for the app to work.
* Executing/running the program via CLI is the most effective way of visualizing it. Spyder, PyCharm has been proven to not work at all or work with minimal functionalities (intermittent crash, program executing once per restarting the environment)

#### Known Bugs

* App crashes when the 'filechooser' widget is given a particular set of inputs (multiple file selection, wrong format file selection etc.)
* App has to be force quit if the program is attempted to stop or perform different tasks when the speech synthesis operation is performing.

Support
=======

If you run into any issues performing the Kivy and KivyMD installation or if the app fails to run, you can ask for help on my mailing list:

* Email: mkabirsh@uwo.ca / mashruk28@gmail.com