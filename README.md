# Mohammad Azeem Khan

**Full-Stack Product Engineer · Geospatial AI · Computer Vision**

I build geospatial products end to end — from the deep-learning model that extracts meaning from imagery to the production system a real user opens and makes decisions from. Based in Salzburg, Austria.

---

## What I Do

I work at the intersection of three things: **geospatial systems**, **computer vision**, and **full-stack product engineering**. As a solo developer, I own products from first principles to production — defining the problem, architecting the solution, building the full stack, and shipping it.

My real interest is the moment raw spatial data — aerial imagery, satellite data, LiDAR — becomes something a planner, regulator, or engineer can actually use to make a decision. That translation is what drives everything I build.

---

## Currently Working On

**TopView — Province-Scale Rooftop PV & Building Detection** *(iSpace Plus, Salzburg)*

End-to-end computer vision pipeline for detecting and segmenting rooftop solar PV installations, building footprints, and outdoor AC units from high-resolution aerial GeoTIFF imagery across Austrian cities.

- Trained and benchmarked **Mask R-CNN (MMDetection)** and **YOLOv8 / YOLO11-seg (Ultralytics)** across 12+ MLflow-tracked experiments on a custom LabelMe-annotated dataset (~3,000 georeferenced tiles at 6 cm GSD)
- Engineered a georeferenced inference pipeline: automated GDAL tiling → model inference → affine-transform-correct mask vectorization → GeoPackage export, scaled to full-city runs for **Graz, Gleisdorf, and Salzburg**
- Published detected layers as QGIS / Lizmap map services for stakeholder review
- Co-authored a peer-reviewed conference paper on the segmentation methodology — **AGIT 2026**

`Python · PyTorch · MMDetection · Ultralytics · GDAL · rasterio · OpenCV · MLflow · QGIS · Lizmap · EPSG:31255/31256`

---

**Strukturdaten Portal — Regulatory GIS Platform for E-Control Austria** *(iSpace Plus, Salzburg)*

Production web portal enabling Austria's electricity and gas regulator to upload, validate, edit, and conflict-check regulatory GIS polygon datasets across competing grid operators (Netzbetreiber). Sole developer, end to end.

- Interactive **MapLibre GL JS (WebGL)** map editor with polygon draw, snap-to-vertex editing, and multi-format ingest (GeoJSON, Shapefile, GPKG) with user-selectable CRS
- PostGIS-driven **auto-clipping engine** (ST_Difference / ST_Intersection) that detects and resolves boundary overlaps within atomic DB transactions — so conflicts can't form in the first place
- Role-based access control (admin / editor / viewer), ownership-scoped CRUD, paginated audit logging with CSV export
- Production infrastructure: Docker Compose · Nginx reverse proxy with TLS · JWT auth with rate limiting · zip-slip-protected uploads · automated security test suite · daily pg_dump backups with grandfather-father-son retention

`Next.js 16 · React 19 · TypeScript · Tailwind CSS · MapLibre GL JS · terra-draw · FastAPI · SQLAlchemy · GeoAlchemy2 · PostGIS · Alembic · Docker · Nginx · Cloudflare Tunnel`

---



## Technical Skills

| Area | Tools & Technologies |
|------|---------------------|
| **Languages** | Python, TypeScript, JavaScript, SQL |
| **Frontend** | React 19, Next.js 16, MapLibre GL JS (WebGL), terra-draw, Tailwind CSS |
| **Backend** | FastAPI, SQLAlchemy, GeoAlchemy2, REST APIs, JWT, OAuth2 |
| **Geospatial** | PostGIS, GDAL, rasterio, QGIS, Lizmap, ArcGIS Pro, Leaflet, OpenLayers |
| **Computer Vision** | PyTorch, Mask R-CNN (MMDetection), YOLOv8/YOLO11-seg (Ultralytics), Instance Segmentation |
| **MLOps** | MLflow, experiment tracking, annotation pipelines (LabelMe), model benchmarking |
| **Infrastructure** | Docker, Nginx, Git, CI/CD (GitHub Actions, Gitea), Linux, Cloudflare Tunnel |
| **Data Formats** | GeoTIFF, GeoPackage, GeoJSON, Shapefile, HDF5, LAS/LAZ |
| **Remote Sensing** | Sentinel-1/2, MODIS, aerial orthophotos, EPSG:31255/31256, WGS84 |
| **AI-Native** | Claude Code CLI, GitHub Copilot, Agentic IDE workflows |

---

## Selected Projects

**Province-Scale Solar PV Detection — Austria**
Detected **10,000+ rooftop solar PV systems across ~7,000 km² of Salzburg province** at ~88% accuracy using instance segmentation on 6 cm GSD aerial imagery. Pipeline scales from raw GeoTIFF to georeferenced GeoPackage vectors ready for cadastre and GIS integration. Multi-city deployment across Graz, Gleisdorf, and Salzburg. AGIT 2026 paper.

**Satellite Imagery Pipeline — EOG GmbH**
Python backend services for automated large-volume retrieval and processing of Sentinel and MODIS satellite imagery, integrated with the Sentinel Hub API (OAuth2). Optimized TIFF/HDF5 storage pipelines serving both interactive visualization and downstream ML inference. Applied deep-learning super-resolution to enhance imagery usability.

---

## Education

**MSc, Geospatial Engineering** — Technical University of Munich *(2020–2023)*
**BTech, Civil Engineering** — Aligarh Muslim University, India *(2015–2019)*

---

## Publications

**AGIT 2026** — Co-author, peer-reviewed conference paper on instance segmentation methodology for rooftop solar PV detection from high-resolution aerial imagery.

---

## Connect

## Links
- GitHub: https://github.com/azeemk210
- LinkedIn: https://www.linkedin.com/in/azeem-khan210/
- Email: khan.azeemak@gmail.com

---

*Austria ·
