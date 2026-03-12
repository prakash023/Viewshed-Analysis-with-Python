==================
VIEWSHED ANALYSIS 
==================

Finds highest mountain peak and shows what areas are visible from it.

REQUIREMENTS:
pip install numpy rasterio matplotlib

FILES NEEDED:
Elevation data (GeoTIFF format). Default path:
I:\sichtbarkeitsanalyse\SRTMGL3.tiff

TO RUN:
python viewshed_analysis.py

OUTPUT:
- Map: visible (green) vs hidden (gray) areas
- Cross-section view of terrain
- Saved as: I:\sichtbarkeitsanalyse\viewshed_result.png

CUSTOMIZE:
- observer_height: change +2 value for taller observer
- clip_deg: analyze larger/smaller area
- step_size: higher = faster but less accurate

TROUBLESHOOTING:
"No module" -> run pip install again
"File not found" -> check file path
Too slow -> increase step_size or decrease clip_deg