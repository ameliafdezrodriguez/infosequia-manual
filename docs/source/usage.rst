========
IS.VH___ & IS.CVIA_
========

Version: 0.1
Document_No.: IS.PUM.VH__/CVIA_
(c) FutureWater
Check at https://docs.typo3.org/m/typo3/docs-how-to-document/main/en-us/GeneralConventions/CodingGuidelines.html 

BAKCGROUND
============

Executive Summary
------------
The IS.VH___ and IS.CVIA_ products include a suite of drought precursors that inform about the health status of vegetation (VH = Vegetation Health) and the greeness dynamics of croplands along the growing season. The VH indices are computed following the VH method proposed by Kogan (1987) from two primary satellite-based indicators: the Normalized Difference Vegetation Index (NDVI), and the Land Surface Temperature (LST), while the CVIA index is based on the evolution of the NDVI seasonal trajectory. Gridded datasets of NDVI are computed from Red and NIR surface reflectance values from MODIS-Terra, OLCI-Sentinel-3 (for NDVI) and SLSTR-Sentinel-3 (for LST) products. Raw datasets are post-processed to denoise the NDVI, and to sharpen the spatial resolution of the NDVI and LST datasets, respectively. For the particular case of the SE3 products, and due to its short time coverage, a synthesis technique is additionally implemented to extend backward the NDVI and LST signals (at least until the same climatology period than for MODIS is covered). Both post-processed datasets, i.e. the denoised NDVI and sharpened LST, are the basis for computing: a) the suite of VH indices, including the Vegetation Condition Index (VCI), the Temperature Condition Index (TCI), and the Vegetation Health Index (VHI), and b) the Cumulative Vegetation Index Anomaly (CVIA). NDVI and LST precursors, and  VH and CVIA indices are computed at dekad (10-day) and monthly resolutions, and at different (1, 3, 6 and 12-month) aggregation timescales. Dekad products are used in InfoSequia for monitoring and visualization purposes, while monthly products are ingested in IS-4CAST processor as forecast predictors. 

Scope and Objectives
------------


Content of the document
------------


REVIEW OF USER REQUIREMENTS
============


ALGORITHM
============

Overview
------------
**This is content of met lot**


Retrieval Methodology
------------


Input data and ingestion procedure
#################
Brief description of:
- MODIS-Terra products
- OLCI-SE3 product
- SLSTR-S3 product

Retrieval of quality-flagged precursors
#################
- NDVI
- LST

NDVI denoising
#################

LST sharpening
#################

SE3 NDVI synthesis
#################


Index calculation
#################




PRODUCT DESCRIPTION
============

File Format and Metadata attributes
------------
Filenaming convention for netCDF outputs: *PPP*.*TT*.*VVVVV*.*SSS*.nc

Product Content
------------

Product Characteristics and Metadata attributes
------------

It includes aspects related with:
- Projection and grid information
- Spatial information
- Temporal information


VALIDATION PROCEDURE
============



PRODUCT USAGE
============

Basic usage
------------


Advanced usage
------------


For example:

>>> import lumache
>>> lumache.get_random_ingredients()
['shells', 'gorgonzola', 'parsley']

