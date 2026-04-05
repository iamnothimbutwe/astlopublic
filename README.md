# astlo

**A real-time and still developing Astronomy/Astrophysics/celestial orbital mechanics engine**
An extensible curently focused on orbital mechanics library for tracking the debris.
CLI + SDK.
Written in pure Python (with future matplotlib/numpy support)

*Copyright © 2026 Macharia [@iamnothimbutwe both on github and gitlab.
*All rights reserved.

*Unauthorized copying, modification, distribution, or commercial use of this software (or substantial portions of it) is strictly prohibited without express written permission from the author.
*License two: another Copyright notice

![Python](https://img.shields.io/badge/Python-3.8%2B-blue)


### Features

- Real-time **barycentric** (SSB) and **heliocentric** position, velocity and gravitational acceleration vectors for **16 bodies**:
  - Mercury, Venus, Earth, Mars, Jupiter, Saturn, Uranus, Neptune, Pluto
  - Ceres, Vesta, Pallas, Hygiea, Haumea, Makemake, Eris
  - real-time position vectors of the Sun relative to the SSB barycenter due to all major planets. Although every celestial object accounts for the SSB.
- **Perifocal (xy)**, **Heliocentric position vectors and position vectors relative SSB.
- Distances in **meters, kilometers, AU**
- **Light delay** (seconds + minutes) from Earth,SSB and Heliocenter
- Orbital velocity using real time velocity vectors relative SSB (m/s and km/s)
- **Mean anomaly** and **Eccentric anomaly**
- Full orbital period animation using **days + AU and seconds + AU**
- **Parallax angle**, distance in **parsecs**, **light years**
- **Specific orbital energy (E)** → automatically classifies orbit type:
  - Circle / Ellipse / Parabola / Hyperbola
- Terminal **orbit plotting** (eccentric orbits) using plotext
- Clean, colored terminal output with tables.


Future plans:
- Full 3D visualization (Z-plane)
- Real-time matplotlib animations
- REST API

### Contacts
- Email markmacgh@gmail.com/hecateare@gmail.com
- Github and Gitlab both @iamnothimbutwe

>...**astlo was and is being developed on Linux from a mobile phone**...

### Project Status
- Pure Python (no numpy,astropy,matplotlib) but numpy will be integrated later..
- Real-time barycentric shifts implemented
- SSB + Heliocentric + perifocal for full periods                     - Terminal plotting with plotext: in some orbits like Eris, Because Er
is has a massive orbital inclination i approx 44°, it is "diving" deep below the ecliptic plane. the program only plots X and Y, you will be looking at the shadow of the orbit, not the actual 3D length. some of the distance is shifted to the Z axis.                               - numpy and matplotlib for Z axis to be integrated later

### Installation

```
??If anyone wants it, contact me and i will send the compiled whl for installation
use pip install 'whl' to install the whl once recieved.
Or go to the releases page for the public repo to astlo and download the release then install using pip install.

or direct download & install from terminal:
pip install https://github.com/iamnothimbutwe/astlopublic/releases/download/v5.61.48/astlo-5.61.48-py3-none-any.whl

download from browser:
https://github.com/iamnothimbutwe/astlopublic/releases/download/v5.61.48/astlo-5.61.48-py3-none-any.whl

    then install the any.whl using pip install astlo-5.61.48-py3-none-any.whl
```

### QUICK Start: SDK & Methods
! [[python IDE](assets/hello.jpg)](assets/hello.jpg)

! [[python IDE](assets/hello2.jpg)](assets/hello2.jpg)

! [[phthon IDE](assets/hello3.jpg)](assests/hello3.jpg)

! [[python IDE](assets/hello4.jpg)](assets/hello4.jpg)
 
! [[python IDE](assets/hello5.jpg)](assets/hello5.jpg)
 
! [[python IDE](assets/hello6.jpg)](assets/hello6.jpg)
 
! [[python IDE](assets/hello7.jpg)](assets/hello7.jpg)
 
! [[python IDE](assets/hello8.jpg)](assets/hello8.jpg)
 
! [[python IDE](assets/hello9.jpg)](assets/hello9.jpg)
 
! [[python IDE](assets/hello10.jpg)](assets/hello10.jpg)
 
! [[python IDE](assets/hello11.jpg)](assets/hello11.jpg)
 
! [[python IDE](assets/hello12.jpg)](assets/hello12.jpg)

! [[python IDE](assets/hello13.jpg)](assets/hello13.jpg)

! [[python IDE](assets/hello14.jpg)](assets/hello14.jpg)

! [[python IDE](assets/hello15.jpg)](assets/hello15.jpg)

! [[python IDE](assets/hello16.jpg)](assets/hello16.jpg)

! [[python IDE](assets/hello17.jpg)](assets/hello17.jpg)

! [[python IDE](assets/hello18.jpg)](assets/hello18.jpg)

! [[python IDE](assets/hello19.jpg)](assets/hello19.jpg)

! [[python IDE](assets/hello20.jpg)](assets/hello20.jpg)

! [[python IDE](assets/hello21.jpg)](assets/hello21.jpg) 

! [[python IDE](assets/hello22.jpg)](assets/hello22.jpg)

! [[python IDE](assets/hello23.jpg)](assets/hello23.jpg)

! [[python IDE](assets/hello24.jpg)](assets/hello24.jpg)

! [[python IDE](assets/hello40.jpg)](assets/hello40.jpg)

! [[python IDE](assets/hello41.jpg)](assets/hello41.jpg)


### CLI: Command Line Interface
! [[terminal](assets/hello25.jpg)](assets/hello25.jpg)

! [[terminal](assets/hello26.jpg)](assets/hello26.jpg)

! [[terminal](assets/hello27.jpg)](assets/hello27.jpg)

! [[terminal](assets/hello28.jpg)](assets/hello28.jpg)

! [[terminal](assets/hello29.jpg)](assets/hello29.jpg)

! [[terminal](assets/hello30.jpg)](assets/hello30.jpg)

! [[terminal](assets/hello31.jpg)](assets/hello31.jpg)

! [[terminal](assets/hello32.jpg)](assets/hello32.jpg)

! [[terminal](assets/hello33.jpg)](assets/hello33.jpg)

! [[terminal](assets/hello34.jpg)](assets/hello34.jpg)

! [[terminal](assets/hello35.jpg)](assets/hello35.jpg)

! [[terminal](assets/hello36.jpg)](assets/hello36.jpg)

! [[terminal](assets/hello37.jpg)](assets/hello37.jpg)

! [[terminal](assets/hello38.jpg)](assets/hello38.jpg)

! [[terminal](assets/hello39.jpg)](assets/hello39.jpg)

### other Features
- full real time Oisculating elements which can be viewed both from the CLI and the SDK through the methods. 
​- heavy Dependencies: 0% external dependencies. Written in pure Python for maximum portability and zero-latency startup in terminal environments (optimized for Termux).
- Epoch: J2000 heliocentric ecliptic
- Custom Bisection/Lambert solver for \Delta V optimization.
- ​Custom Ephemeris: No SPICE kernels required. High-precision position and velocity vectors calculated from custom-built analytical models.
​Independence: No astropy or numpy in the core engine. All 64-bit vector math is handled via internal classes.
- ​CLI Visualization: Real-time orbital plotting rendered directly in the terminal without matplotlib.CLI-based ASCII/Block rendering for real-time orbital plotting (Optimized for Termux/VT100).
### ​🛠 Evolution (Roadmap)
- ​While the core remains "Silent and Light," astlo is evolving to handle high-complexity simulations.
- ​Hybrid Integration: Optional numpy support for 3D state-vector arrays and Delta V optimizations.
- ​Launch Simulations: Integrating atmospheric drag and multi-stage thrust profiles.
- ​Advanced Visuals: matplotlib and vpython hooks for 3D orbital animations and launch-to-intercept visualizations.
