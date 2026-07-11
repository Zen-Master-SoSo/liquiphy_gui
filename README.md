# liquiphy_gui

A quick and dirty GUI interface to the liquidsfz command-line using python's subprocess.

Need to listen to an .sfz file without a lot of hassle? Use liquiphy_gui!

	$ liquiphy-gui <path-to-sfz>

The above command loads the given .sfz file in a liquidsfz instance and
automatically connects the Jack MIDI input and Jack audio outputs to the first
available (physical) ports, displaying the SFZ name and ports connected in a
simple dialog.

<img width="400" height="168" alt="Main tab" src="https://github.com/user-attachments/assets/43290c38-9549-4978-b639-d6886e5d5154" />

Errors that liquidsfsz reported during parsing show up in the "Errors" tab:

<img width="400" height="168" alt="Errors tab" src="https://github.com/user-attachments/assets/c1c2a6e1-a850-40db-8703-b067078aa77c" />


Hit the Escape key or ctrl-Q to exit.

## Install

You must install liquidsfz first for this package to work. To install:

	$ git clone https://github.com/swesterfeld/liquidsfz.git

Follow the instructions found in the liquidsfz README to install liquidsfz.

Install this package (liquiphy_gui) using python pip:

	$ pip install liquiphy_gui

...or...

	$ python3 -m pip install liquiphy_gui

## File associations

If you would like to open .sfz files in liquiphy-gui by double-clicking them in
your file explorer, you can add an association.

1. Right click on an .sfz file to bring up the context menu.

2. Select "Open With", and then "Other Application"
<img width="799" height="525" alt="nemo-open-with" src="https://github.com/user-attachments/assets/b203be50-ca67-44e1-8511-b50569071541" />

3. In the dialog show, look for "liquiphy-gui" in the list of applications, and
then click "Set as default".
<img width="575" height="563" alt="gnome-set-default" src="https://github.com/user-attachments/assets/cd1c7bea-f867-475e-afee-b11451a3fd55" />


Now, all it takes to preview an .sfz is double-clicking on it. Jack ports are
instantly connected, and you have your live preview.
