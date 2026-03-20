# **Coronal Hole Detection and Magnetic Flux Analysis**

## **Overview**
This project provides a Python workflow to identify coronal hole (CH) boundaries from **AIA 193 Å EUV images** and estimate their magnetic properties using co-aligned **HMI magnetograms**. It focuses on measuring CH area and calculating total unsigned magnetic flux for space weather–related studies.

---

## **Method**
The code normalizes AIA images using exposure time and reprojects them to the HMI coordinate system. A region of interest is selected, and coronal holes are detected using intensity thresholding with smoothing. The largest connected region is identified as the CH, and its boundary is extracted. This boundary is then applied to the magnetogram to isolate the corresponding magnetic field. Area and total unsigned magnetic flux are computed from the masked region.

---

## **Requirements**
- Python 3.x  
- NumPy  
- SciPy  
- Matplotlib  
- SunPy  
- Astropy  
- scikit-image  
- aiapy  

---

## **Usage**
1. Provide **AIA 193 Å** and **HMI FITS files**.  
2. Run the notebook step by step, adjusting threshold parameters if needed.  
3. Outputs include CH boundaries, masked magnetograms, area estimates, and magnetic flux values.

---

## **Output**
- Coronal hole maps  
- Boundary overlays  
- Masked magnetic field data  
- Calculated area and flux  

---

## **Author**
**Bhairab Ale**  
MSc Physics, Central Department of Physics, Tribhuvan University, Kirtipur, 44613, Nepal

---

## **Acknowledgements**
This project was inspired by and adapted from the GitHub repository: [**katuwal13/Paper_Coronal_hole_2025**](https://github.com/katuwal13/Paper_Coronal_hole_2025).

---

## **Notes**
Intended for research use; results may vary depending on data quality and parameter selection.
