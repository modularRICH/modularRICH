# Modular Ring Imaging Cherenkov Particle Identification Detector
The modular aerogel RICH is designed for hadron identification covering a momentum range of 3-10 GeV/c. Identification of the hadrons in the final state is needed for understanding how different quark flavors contribute to the properties of hadrons, and reliable identification of the scattered electron is important for covering kinematics where pion backgrounds are large. This hardware is being prototyped as one of the detectors in the future [Electron-Ion Collider](https://arxiv.org/abs/1212.1701) (EIC), and some of them have recently been tested at Fermilab.

![][modularRICHiso]

## Theory
Aerogel, silicon dioxide and air has a very low index of refraction, and is being used as a radiator material. When high energy charged particles, the remnants of collisions in the interaction region, pass through the aerogel, their phase velocity exceeds that of the speed of light in the medium. The release some of this energy in the form of cones of light, emanating from the collision point. The particle continues through, generally passing through the rest of the instrument.

This cone of light then passes through the Fresnel lens where it is focused towards the center of the sensor plane, which lies at the focal length. The mirrors provide light from particles coming in at an angle to still be focused on the sensor. The ring pattern that emerges can be able to differentiate pions and kaons, and their respective energies.

![][gemc]

## Hardware
The detector consists of a optical cavity that is sealed to be light tight, and a interface board for electronics, that allows the heat to be dissipated. The modules are designed to be easily removable allowing runs with and without the mirror, aerogel, and/or lens.  The list follows the beam path.

![][explodedIsoA]

### Frame
The frame is made from 1/4" aluminium and assembled with 4-40 screws. The flat butt joints allow flat gaskets to be sandwiched between the sections if needed. The metal sides are much better at blocking light than the acrylic used before that was less opaque than expected. The top and bottom sections are grooved allowing precise placements of the inner modules, and prevent them from shifting. Any of the five panels can be easily removed with only four screws, making servicing quick.

![][closed]

### Aerogel
Silica aerogel has been used for decades in threshold Cherenkov counters for high energy physics. The aerogel block used is 110mm x 110mm x 33mm and housed in a foam block. The material is extremely fragile and fractures irregular based on formation impurities. It has a index of refraction around 1.01-1.10 depending on its quality, and may have a slight blue hue or be completely clear.

![][pmtExploded]

### Fresnel Lens
The fresnel lens used in this design is manufactured by Edmond Optics [32-593](http://www.edmundoptics.com/optics/optical-lenses/fresnel-lenses/fresnel-lenses/32593/) and has the critical dimension of 3in for the focal length. It is cut smaller than its original 6.7in x 6.7in on order to fit the box, and has an effective diameter of 6in. Due to those two factors, the edges of the lens do not contain any grooves, and are ineffective at refracting light.

![][fresnelLens]

### Mirror
The mirrors used are front surface mirrors that are trapezoidal. Four of these assemble into a pyramid with a wall inclination of 5 degrees. They are scientific grade 6mm glass mirrors purchased from [fsm](http://firstsurfacemirror.com/trapezoid-first-surface-mirror/) who provides cutting to size. They are glued into acrylic holders that also act as spacers providing exactly the focal length between the lens, and the sensor.

![][pmtExploded]

### Sensor
The sensor is the method of readout for determining ring size. As the number of photons produced is low, and event rate is high, the option used in the first prototype was a anode photomultiplier tube (pmt) array [H12700](https://www.hamamatsu.com/resources/pdf/etd/H12700_TPMH1348E.pdf) a 8x8 pixel (6mm x 6mm pixel size) pmt array. A new option of using MPPC arrays is being considered as a smaller pixel size (3mm x 3mm is required for energy range differentiation).

![][backMPPC]

#### MPPC
3mm x 3mm pixel size in a 8x8 array is being considered with 16 modules, meaning 1024 channels being required to act as the sensor plane. Each 8x8 module connects to a backplane that breaks the electrical signals out, allowing electronics to be mounted on the back.

![][mppcDetail]

#### PMT
A 16x16 PMT array with a 3mm x 3mm pixel size is another option. This yields the same coverage area, and the same number of signals, but presents a thicker profile as the dynodes in a PMT require separation. The contacts of this sensor are also broken out through the PCB.

![][pmtSide]

[backMPPC]: renderings/backMPPC.jpg "View of Back of Board"
[closed]: renderings/closed.png "View of Back of Board"
[explodedIsoA]: renderings/explodedIsoA.jpg "View of Back of Board"
[fresnelLens]: renderings/fresnelLens.jpg "Detail view of Fresnel Lens"
[modularRICHiso]: renderings/modularRICHiso.jpg "View of Back of Board"
[gemc]: renderings/gemc.jpg "View of Back of Board"
[mppcDetail]: renderings/mppcDetail.jpg "View of Back of Board"
[pmtExploded]: renderings/pmtExploded.jpg "View of Back of Board"
[pmtIsoB]: renderings/pmtIsoB.jpg "View of Back of Board"
[pmtSide]: renderings/pmtSide.jpg "View of Back of Board"
