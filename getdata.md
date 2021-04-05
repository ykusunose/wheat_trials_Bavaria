# Get 2010 GVE density (?)

https://www.wcs.nrw.de/stba/agraratlas?REQUEST=GetCoverage&SERVICE=wcs&VERSION=1.0.0&CRS=EPSG:4326&BBOX=5,46,16,56&COVERAGE=K05_GVEdichte_2010&WIDTH=5000&HEIGHT=5000&FORMAT=GeoTIFF

# Make tile layer

gdal2tiles.py -p mercator -z 1-9 -w all -r average -a 0.0 /Users/boyd/Downloads/gve-density.tif /Users/boyd/Downloads/temp

Five classes are shown but don't know what they represent