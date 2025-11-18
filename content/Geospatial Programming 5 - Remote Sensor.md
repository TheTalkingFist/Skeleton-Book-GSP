
Remote sensing is the science of obtaining the physical properties of an area without being there, hence, "remote".

It allows users to capture, visualise and analyse objects and features on Earth's surface. By collecting imagery, we can classify it into land cover and other types of analyses.

---
## Sensor Types

These are applications of Remote-Sensing

- Unmanned Aerial Vehicles (UAV) and Drones
	- Advantages:
		- Provides high-res images
		- Paths of flight can be programmed
		- Comes with LIDAR
	- Disadvantages:
		- Covers a small area
		- Small visual LOS
- Airplanes and Helicopters
	- Advantages:
		- High-res images
		- Planned paths
		- Comes with LIDAR
	- Disadvantages
		- Small coverage extent
		- Requires flight operation
- Low Earth Orbit Satellites
	- Advantages:
		- High to coarse resolution images
		- Large coverage
	- Disadvantages:
		- Coverage is limited to its path of orbit
		- Vulnerable to cloud obstructions




---

# Image Resolution

## Spatial Resolution
The detail in pixels of an image. High spatial resolution means more detail and smaller pixel size, and opposites. 

## Spectral Resolution
Amount of spectral detail in a band. High-spectral-res means bands are more narrow, while lower-res means bands are wider and cover more of the spectrum.

## Temporal Resolution
Time it takes for satellite to complete a full orbit. Drones and planes are okay with this, but they have small coverage.

GPS satellites are in medium-earth orbit (MEO). Because they follow a continual orbit, revisit times are constant.

Let's put this in a GPS context. A good GPS would update frequently, which it does by the satellite revisiting the same place multiple times frequently. Therefore, a good GPS would have a high temporal resolution

---
# Types of Orbits

Three types of orbits:
- Geostationary orbits match Earth's rotation
- Sun-synchronous orbits keep the angle of sunlight on earth as consistent as possible
- Polar orbits pass above or nearly above both poles of Earth

It's the satellite's height above the Earth's surface that determines the time it takes for one complete orbit. Intuitively, the higher the altitude, the longer the orbital period.

As we know, Medium Earth Orbits (MEO) are mostly used for GPS'. In High Earth Orbit, we have weather, comms and surveillance satellites. CubeSats and the ISS are in Low Earth Orbit.

---
# Types of Remote Sensing

## Passive sensors
Measures reflected light emitted from the sun. When the sunlight reflects off of the Earth's surface, passive sensors capture it. Our eyes are a form of passive sensors.

The Landsat and Sentinel satellites are passive sensors.

## Active sensors
Sends out signals to targets and receives the reflection, measuring it. Kinda like radars. The signal is called a pulse, and the reflection a backscatter.

An example of active sensors are Radars and Sonars.

---

# Local Issues

We usually use UAVs, helicopters and airplanes for local issues. Not to say satellites are useless.

Examples include:
- **Li**ght **D**etection **a**nd **R**anging (LIDAR)
	- Building topographic models on the ground
- **So**und **Na**vigation **R**anging (Sonar)
	- Building topographic models underwater
- Radiometers (measures heat) and Spectrometers (measures electromagnetism)

# Global Issues

Satellites usually handle the global ones.

- Navigating with GPS
- Climate change monitoring
- Arctic surveillance

---
Next:
[[Geospatial Programming 6 - Data Model, Attribute Management]]

Prev:
[[Geospatial Programming 4 - Geographic Information System (GIS)]]

Index:
[[0 - Intro]]