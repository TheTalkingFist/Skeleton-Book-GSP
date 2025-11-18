
This is a multi-component environment meant to create, visualise and analyse data and spatial counterparts. Most datasets encountered will can all be assigned a spatial location, weather on Earth's surface or within arbitrary coordinates.

For example, if we had a table that ranks countries based on some variable, we can use GIS to visualise that data better by perhaps coloring each country on a map with a shade of green, where a darker shade means a higher intensity or value of the variable.

---
## Spatial Analysis

Imagine you recorded the location of each tree in a well-defined study area, then map the location of each tree. At this point, you'd probably start seeing patterns, and in turn make inferences based on what you see.

![[Pasted image 20251117211218.png]]

In short; you will be able to find out more information by mapping.

In the context of the above example, we can see that maybe not all areas are equally dense with trees, with some places having far less trees than others. This could then lead us to question the quality of soil. We went from trees to soil quality.


To put this all into perspective, we can take the road, carpark and bus stop labsheet as an example:
1. The GeoData is the map that we got, that we used as a base
2. The GIS is the tool we used, which in this case, is QGIS
3. Spatial Analysis is the end product, as in the screenshot of the GeoData with annotated roads, carparks and bus stops

---

## Coordinate Reference System (CRS)

As we know, Earth is a sphere. But, not really. It bulges at the equator, and is way less smooth than... smooth.

The reason our globes are visualised as being smooth is because of coordinates, or, the Coordinate Reference System (CRS).

CRS is a framework of defining real-world locations based on a globe model.

There are two types of CRS:
1. **Geographic Coordinate System**
2. **Projected Coordinate System**

So, how do we go from a weird, not-really-ball-shaped ball to a ball, or even a flat map?

### GCS, Data and Datum
A datum is a model that has the following:
1. Angular units (i.e degrees)
2. A starting point (0, 0), and
3. A defined position of the spheroid, relative to the centre of the earth (Also happens to be the origin orientation for latitude and longitude lines)

All of these add up to GeoData, which is the sum of Data and Data Description.
![[GeoData Chart.png]]

Note the "GCS - Defined by a Datum".
![[European Datum.png]]

~~We will use this as an example. This image shows two different conflicting datums.~~

~~They both have Angular units. They also have a starting position (0, 0) where the two perpendicular lines meet.~~

~~You can see the starting position for both datums is different.~~ 


---
## Projected Coordinate Systems

Earth is flat!

No, it's not. But, we can project Earth's very non-flat mapping onto a flat plane.

It's a reference systems for identifying locations and measuring features on flap (map) plane.

There are a few ways to do this.

### Planar Projections
<sub>Azimuth: The horizontal angle from a cardinal direction, most commonly north, in a local or observer-centric spherical coordinate system.</sub>

This maps the surface of our Terra to a flat surface that touches earth's surface at a point (tangent case) {...whatever that means}

This one is often used for mapping polar regions, but can be used on any location (and those are called Oblique Planar Projections)

The final map will look circular, similar to the UN logo.

### Cylindrical Projection

This maps the earth surface onto a map, rolled into a cylinder which can then be flattened to a real plane. The cylinder can touch the surface of the earth a long a single line of tangency (a tangent case).

This is the most popular method of projection. If you've seen a map on a wall, then it very likely used this method. In fact, it's called the Mercator projection.

While the linear scale is equal in all directions around any point, some of the sizes do get distorted as latitude increases from equator to the poles where, in theory, scale becomes infinite. Math is weird.

### Conical Projection

As you can probably guess, this maps the earth's surface onto a map rolled into a cone which can touch the surface along a single line of tangency (you know the story by now).

With this one, distortion is minimised along the tangent or secant lines. It does increase when we get further from them, though.

When distance or area measurements are needed for the 48 states, use one of the conical projections, Equidistant Conic (preserves True Distance) or Albers Equal Area Conic (preserves True Area). These are popular in European maps.


As with most things in life, choosing a projection method is a compromise. A map can have one, or maybe more than one for small locations, but never all of these properties:
- True Area
- True Distortion
- True Distances
- True Shapes

In this case, "True" means that they retain the same properties or appearance as they do on a real globe. When choosing a map, we will need to stick with one or more of these pros, but never all. There is no "best projection", just the one that works for whatever your cause is.

---
Here are some common projections:

- The Robinson Projection, by Arthur H. Robinson
	- This is a map projection of a world map that shows the entire world at once. It was made in an attempt to find a good compromise to the problem of showing the globe as a flat image.
- Gall-Peters Projection, by James Gall and Arno Peters
	- This is a rectangular, equal-area map projections that still distorts shapes.

---
Next:
[[Geospatial Programming 5 - Remote Sensor]]

Prev:
[[Geospatial Programming 3 - Introduction to GeoBIM]]

Index:
[[0 - Intro]]