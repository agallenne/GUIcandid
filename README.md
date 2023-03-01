# [C]ompanion [A]nalysis and [N]on-[D]etection in [I]nterferometric [D]ata

This is a PyQT5 Graphical user interface for the CANDID algorithm to find faint companion around star in interferometric data in the OIFITS format. This tool allows to systematically search for faint companions in OIFITS data, and if not found, estimates the detection limit. This code is presented in the article [Gallenne et al. 2015](https://ui.adsabs.harvard.edu/abs/2015A%26A...579A..68G/abstract), although it has evolved slightly since the paper was published.

CANDID code/install/examples can be find in the original repository [here](https://github.com/amerand/CANDID). A CANDID version is also available here with some new features:

      - Can save in FITS format the nsigma detection level map for further purposes
      - Can select the nsigma threshold (default=3)
      - The bootstrap function now also provides the astrometric error ellipse
      - Can select a spectral range
      - Can display the N best detections
      - Can add some binary parameters (Porb, ecc, MT and distance) as imput in fitMap
        to directly estimate the maximum search (if known spectroscopic binary). NOT
        IMPLEMENTED IN THE GUI YET
      - Can set a region to search instead of (0,0) 
      
To run the GUI, go to the directory then type:

```
GUIcandid 
```

The GUI will open. Tool tips are available with some explanations of each function.

Note: Only tested on MacOS 13.12 with Python 3.8.13 and Ubuntu 22.04.1 with Python 3.9.13

![GUI](https://user-images.githubusercontent.com/12450258/222246116-fa1d7582-15df-4b0b-9308-fb272027de68.png)
