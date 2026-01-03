# Cemetery Burial Records GIS Visualization

This repository contains a complete workflow for converting raw cemetery burial records into a structured GIS dataset and high-quality cartographic maps using **QGIS**.

The project demonstrates data cleaning, spatial data preparation, coordinate handling, rendering optimization, and map layout production suitable for academic, archival, or digital humanities use cases.

---

## 📌 Project Overview

- **Dataset**: Cemetery burial records (CSV)
- **Study Area**: Mountain View Cemetery, Vancouver
- **Coordinate System**: WGS 84 (EPSG:4326)
- **GIS Software**: QGIS
- **Output**: Publication-ready maps (overview & detailed scale)

This project focuses on transforming non-spatial tabular data into accurate spatial point data and presenting it efficiently despite large feature counts.

---

## 📂 Repository Structure

```text
cemetery-gis-data-conversion/
├── data/
│   ├── raw/
│   │   └── cemetery_records_raw.csv
│   └── processed/
│       └── cemetery_records_working.csv
│
├── qgis/
│   ├── cemetery_project.qgz
│   └── cemetery_layout.qpt
│
├── output/
│   ├── cemetery_overview_map.png
│   ├── cemetery_detail_map_1200.png
│   └── cemetery_layout.pdf
│
└── README.md 
```

## 🧹 Data Preparation Steps

1. **Cleaned date fields**
   - Standardized date format to `YYYY-MM-DD`
   - Identified missing or unknown dates
2. **Validated attributes**
   - Checked null values and formatting errors
3. **Prepared spatial fields**
   - Latitude and longitude fields validated
   - Geometry generated as point features

---

## 🌍 Spatial Processing

- Imported CSV as **Delimited Text Layer**
- Geometry created using:
  - Latitude → Y field  
  - Longitude → X field
- CRS explicitly set to **EPSG:4326 (WGS 84)**
- Geometry verified and rendered correctly in QGIS

---

## 🎨 Cartographic Design

### Symbology
- Simple marker symbols
- Optimized marker size for high-density points
- Consistent color scheme for clarity

### Performance Optimization
- Rendering order optimized
- Labels minimized for performance
- Layer rendering simplified for layout export

---

## 🗺️ Map Outputs

The project includes two main map products:

1. **Overview Map**
   - Displays the full cemetery extent
   - Suitable for contextual understanding

2. **Detailed Map (Scale ~1:1200)**
   - Focuses on burial block-level detail
   - Suitable for archival reference and close inspection

Both maps include:
- Title
- Legend
- Scale bar
- North arrow

---

## 📤 Export Settings

- **Image Export**: PNG, 300 DPI
- **Document Export**: PDF (non-georeferenced for performance)
- Optimized to avoid clipping, missing features, or rendering delays

---

## 🛠 Tools & Technologies

- **QGIS** (Spatial processing & cartography)
- **CSV / Excel** (Data preparation)
- **WGS 84 CRS** (Geographic coordinate system)

---

## 📚 Use Cases

- GIS portfolio demonstration
- Academic coursework
- Digital humanities projects
- Cemetery and heritage mapping
- Large point dataset visualization

---

## 📄 License

This project uses publicly available open data.  
Please refer to the original data provider’s license for reuse conditions.

---

## 👤 Author

**Samueli wINDOVADO Fau**  
GIS & Spatial Data Enthusiast  
Focus areas: GIS, Remote Sensing, Spatial Data Processing

---

