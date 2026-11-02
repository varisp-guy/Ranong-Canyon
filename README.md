# Ranong-Canyon
An interactive 3D site atlas of Ranong Canyon, a post-extractive pond site in Ranong, Thailand.

## What it shows

- **Topography:** a translucent triangulated mesh with a point texture, cropped from a 5 km Rhino model to the area around the pond.
- **Water:** the pond surface at 50% opacity.
- **Contours and road:** 5 m contour lines and the road network.
- **Trees:** 5,407 *Ficus religiosa* placed at surveyed tree points, drawn as black silhouettes with a white outline.
- **Siltation model:** a 0–20 year simulation of soil moving downslope into the pond. It shows deposition, erosion, the shoreline at each year, and a readout of pond area, volume and net fill.
- **Exploded view:** every layer separates vertically for independent viewing, with the combined site layer at the bottom.

## Siltation model

The model uses slope-driven soil transport and conserves soil: whatever leaves a slope is deposited downslope or in the pond. The default rate is a placeholder, so the results are **uncalibrated** and should be read as a scenario, not a forecast. Set the rate slider to match local observations of how fast the shoreline has moved.

## Data

- Source geometry is exported from Rhino: topography mesh (OBJ), water (OBJ), contours and road (DXF), and tree points (CSV).
- The geometry is processed in Python, then embedded in the page.
- Built with [three.js](https://threejs.org) r128, loaded from a CDN, so the page needs an internet connection.
