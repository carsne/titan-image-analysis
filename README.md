# Titan Atmosphere Image Analysis

This project processes and analyzes images from NASA’s Cassini Imaging Science Subsystem (ISS) to investigate seasonal atmospheric changes on Titan, Saturn’s largest moon.

We map and geometrically correct raw spacecraft images, then apply edge detection to identify the boundary between Titan's brighter and darker hemispheres. The orientation of this boundary relative to the planet’s rotation axis provides insight into atmospheric tilt and variability.

📄 **Related Publication**:  
[Titan's Atmospheric Albedo Asymmetry and Seasonal Variability Observed through the Cassini Imaging Science Subsystem](https://iopscience.iop.org/article/10.3847/PSJ/ad0bec) (The Planetary Science Journal)

---

## Features

- ISIS3-based preprocessing pipeline (via PySIS)
- Geometry correction using SPICE kernels
- Edge detection using `scikit-image` and `OpenCV`
- Angle estimation of hemispheric boundary relative to Titan’s axis
- Visualization of boundary evolution over time

---

## Technologies & Tools

- **Python**, **PySIS**, **ISIS3**
- **OpenCV**, **scikit-image**, **Matplotlib**
- **Astropy**, **scipy**, **skspatial**
- Data Source: [NASA PDS OPUS3 Search Tool](https://opus.pds-rings.seti.org/opus)
