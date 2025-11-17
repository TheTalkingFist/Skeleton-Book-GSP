# Geo(spatial) data
Data, with descriptions... yeah.

It can be converted into vector and raster.

From the labsheets, we know there are 3 ways to represent data.

1. Points
	1. Simple XY coordinates, zero-dimensional
	2. Bus stops, trees, lampposts, etc.
2. Line
	1. A series of points connected by a line, one-dimensional
	2. Rivers, roads, canals
3. Polygons
	1. A set of joint vertices in a particular order that forms an enclosure, two-dimensional
	2. Buildings, car-parks

---
# Modifiable Areal Unit Problem (MAUP)

This is a statistical bias that occurs when you aggregate point data. The two types of biases are:
- Scale effect
- Zonal effect

The result of spatial analysis can vary, based on delineation of geographic units.

Essentially, different conclusions can occur when we use different units over an area, or divide it by a greater or lesser amount.

## Zonal Effect
Occurs when you group data by various artifical boundaries. Essentially, you can get different results when you divide a country by counties and states.

The practical difference between the two is kinda really just shape. Scale depends on specific unit squares, while zonal depends on boundaries.

---
# Raster Data Model

A representation of the world through a matrix of cells/pixels, organised into rows and columns (a grid, basically). Each pixel contains a value and can be continuous (elevation) or discrete/categorical (land use).

## Vector vs. Raster

| Raster                                  | Vector                             |
| --------------------------------------- | ---------------------------------- |
| Difficult to make overlays              | Easy to make overlays              |
| Difficult to register, scale, reproject | Easy to register, scale, reproject |
| Large files                             | Small files                        |
| Difficult to update                     | Network analysis                   |
| Continuous features                     | Discreet features                  |
| Sensor data                             | GPS data                           |
| -                                       | Easier to update                   |

It's important to keep in mind that a perfect representation of the world is impossible, and what is "accurate" is dependent on you and your intended purpose for the map.

---
# Attribute Data Management

Attributes are descriptive information related to an object, often displayed in table format (CSV) or in a database management system. For example, an HDB flat may have coordinates, polygons and stuff like postal code and the block number.

## Types of Attributes
And it all comes back to programming.
- Integers
- Floats/Real
- Test/String
- Date
To be honest, these all look quite self-explanatory.

## Measurement Level of Attributes

![[Pasted image 20251117221011.png]]

---
Next:
[[Geospatial Programming 7 - Geocoding]]

Prev:
[[Geospatial Programming 5 - Remote Sensor]]

Index:
[[0 - Intro]]