
# 🌈 Spectral Rendering

**Rendered Multispectral 3D Scenes Using Physical Illumination Models**

This project demonstrates physically-based spectral rendering using **spectral reflectance**, **spectral power distributions (SPDs)**, and **camera spectral sensitivity models**. The goal is to explore how varying illumination conditions impact the appearance of materials and the accuracy of color reproduction.

<p align="center">
  <img src="images/bmw-m6.png" alt="Rendered BMW M6" width="60%">
</p>

---

## 🔬 Project Highlights

- **Spectral Rendering Pipeline** built with [PBRT](https://pbrt.org/), Blender, and Python.
- **Custom Materials** designed using spectral BRDFs and real-world reflectance data.
- **Illuminants** modeled via real spectral power distributions (D65, Tungsten, etc.).
- **Camera Simulation** based on spectral sensitivity curves for realistic capture.
- **Experiments** conducted to evaluate material appearance shifts under different lighting.

---

## 🗂 Repository Structure

```bash
Spectral-Rendering/
│
├── materials/         # Material definitions with spectral BRDFs
├── textures/          # Texture maps used in scenes
├── reflectance/       # Measured reflectance spectra
├── spds/              # Spectral Power Distributions of illuminants
├── geometry/          # Geometry and models (e.g., BMW M6)
├── experiments/       # Scene files with different material and light settings
├── images/            # Output renders and visualizations
├── .gitignore
├── BLENDSWAP_LICENSE.txt
├── README.md
└── *.pbrt             # PBRT scene configuration files
```

---

## 🛠 Tools & Frameworks

- [PBRT-v3/v4](https://github.com/mmp/pbrt-v3): Physically based rendering toolkit
- [Blender](https://www.blender.org/): Geometry modeling and export
- Python: For data preprocessing and automation
- NumPy, Matplotlib: Spectral data manipulation and visualization

---

## 🚀 Getting Started

1. **Install PBRT** (v3 or v4) from [official repo](https://github.com/mmp/pbrt-v3).
2. Clone this repository:
   ```bash
   git clone https://github.com/huynhtruc0309/Spectral-Rendering.git
   cd Spectral-Rendering
   ```
3. Modify or create your own `.pbrt` scene files using provided materials and SPDs.
4. Run PBRT:
   ```bash
   pbrt bmw-m6-dragon_250.pbrt
   ```
5. Visualize output images and compare spectral effects.

---

## 📊 Sample Results

| Illuminant      | Material: Gold Coating      |
|-----------------|-----------------------------|
| D65             | ![D65](images/bmw-m6.png)   |
| Tungsten        | *(example render here)*     |
| Fluorescent     | *(example render here)*     |

---

## 📄 License

Geometry and assets from BlendSwap licensed under [Creative Commons](https://www.blendswap.com/blends/view/69738).  
Other code and assets are for educational and non-commercial use only.

---

## ✍️ Author

**Jennie Truc Huynh**  
Master's in Computational Colour and Spectral Imaging  
[GitHub Profile](https://github.com/huynhtruc0309)
