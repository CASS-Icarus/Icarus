# Icarus

I. DATASET CATEGORIES

Solar-Panel Surface Imagery
RGB, IR, thermal
Dust/sand accumulation levels
Panel defects (cracks, hotspots)
Clean vs. dirty comparative datasets
Dust / Sand / Soiling Detection Datasets
Aerial/ground images of dusty surfaces
Surface contamination datasets
Agricultural soil/dust segmentation datasets
Robotics Perception & Navigation
Edge detection
Few-shot navigation
Obstacle detection
SLAM datasets
Terrain classification (smooth, slippery, uneven)
Solar Photovoltaic (PV) Performance Time-Series
AC/DC power output
Irradiance, temperature, wind, humidity
Soiling ratio datasets
Maintenance logs
Environmental Dust & Weather Forecasting
Atmospheric dust concentration
Sandstorm historical data
Air quality datasets
Satellite-based aerosols (AOD)
Battery, Power Management & Energy Storage
Battery degradation datasets
Charging-discharging cycles
Robot duty-cycle datasets (analogous to mobile robots)
Mechanical Component / Brush Wear Datasets
Time-to-failure datasets
Vibration signatures
Rotational load changes
Maintenance logs (open-source industrial datasets)
Robotics Docking & Recharging Datasets
Autonomous docking datasets
Localization & fiducial marker datasets
Obstacle Detection (Solar Farm Environment)
Ground robots
Terrain segmentation
Structural recognition (panel frame edges, junction boxes)
Synthetic & Simulation-Based Datasets
Gazebo / Isaac Sim robot models
Synthetic dust rendering
Reflectance models

II. DETAILED DATASET LIST

Below are the best datasets for each category with name, link, description, license, and robot relevance.
1. Solar Panel Imagery
1.1 PV-IR / PV RGB / PV Defect Datasets

Solar Panel Surface Defect Dataset (RGB)
Link: https://github.com/darshanbagul/Solar-Panel-Images

License: MIT
Description: RGB dataset of panels with dust, cracks, hotspots.
Why useful: Contains dust-class images and real-world contamination examples.
EL PV Defect Dataset (Electroluminescence)
Link: https://github.com/zae-bayern/elpv-dataset

License: CC BY-NC-SA
Description: High-res EL imagery of PV cell failures.
Why useful: Helps train models distinguishing dirt vs. cell damage.
Thermal Solar Panel Dataset
Link: https://zenodo.org/record/7784523

License: CC BY
Description: Thermal imagery of PV modules with anomalies.
Why useful: Thermal contrast can detect dirt-induced hotspots.

2. Dust / Sand / Soiling Detection
2.1 Soiling Detection from PV Research

PV Soiling & Cleaning Dataset (NREL)
Link: https://data.nrel.gov/submissions/199

License: ODC-By
Description: Time-series power drop, soiling ratios, weather.
Why useful: Gold-standard for correlating dirt & power loss.

2.2 Environmental / Dust Surface Segmentation
Desert Scene Dataset (Saudi Arabia DESD)
Link: https://github.com/ksu-cv/desert-dataset

License: CC BY-NC
Description: High-res desert surface images.
Why useful: Provides textures of dust that resemble soiling on panels.
SoilNet Dataset
Link: https://vision.eng.au.dk/soilnet

License: CC BY
Description: Soil segmentation dataset (10k images).
Why useful: Train dust segmentation for close-up panel images.
Aerial Dust/Surface Dataset – DeepGlobe Land Cover
Link: https://www.kaggle.com/datasets/crowdflower/deepglobe-land-cover

License: CC0
Description: Land cover classification with sandy classes.
Why useful: Useful for environment modeling and dust context.

3. Robotics & Navigation
3.1 Edge Detection & Obstacle Segmentation
NYU Depth V2
Link: https://cs.nyu.edu/~silberman/datasets/nyu_depth_v2.html

License: Non-commercial
Description: RGB-D indoor images with edges and obstacles.
Why useful: Training edge-detection for panel frames.
BSDS500 – Boundary Detection Dataset
Link: https://www2.eecs.berkeley.edu/Research/Projects/CS/vision/grouping/resources.html
License: BSD
Why useful: Best dataset for edge detection networks.

3.2 Autonomous Navigation / SLAM
KITTI Vision Benchmark Suite
Link: http://www.cvlibs.net/datasets/kitti/

License: CC BY-NC-SA
Why useful: Obstacle detection, depth estimation—robot may need these for navigating panel rows.
TUM RGB-D
Link: https://vision.in.tum.de/data/datasets/rgbd-dataset
License: CC BY-SA
Why useful: SLAM benchmarks useful for robot docking localization.
ETHZ MAV Dataset
Link: https://projects.asl.ethz.ch/datasets

License: Varies
Why useful: Visual-inertial navigation similar to rooftop terrain.

4. PV Performance & Time-Series
4.1 Performance vs Dirt / Weather

NREL Soiling & Performance Dataset
(link above)
Why useful: Combines power, soiling, cleaning events — perfect for predicting cleaning need.
Solar Radiation Data (NSRDB)
Link: https://nsrdb.nrel.gov

License: Free public use
Why useful: Irradiance & weather needed for energy drop estimation.
Open Power System Data (OPSD)
Link: https://open-power-system-data.org
License: MIT
Why useful: Time-series energy production trends.

4.2 Atmospheric Dust (AOD)
NASA MODIS Aerosol Optical Depth (AOD)
Link: https://modis.gsfc.nasa.gov/data/dataprod/mod04.php
License: Public
Why useful: Sandstorm prediction → dirt accumulation forecasting.
CAMS Global Atmospheric Composition
Link: https://ads.atmosphere.copernicus.eu

License: Free
Why: Dust concentration + deposition rates.

5. Environmental / Desert Conditions
5.1 Open Desert / Arid Terrains
Sahara Desert Dataset
Link: https://www.kaggle.com/datasets/nikitarom/sahara-dataset

License: CC
Why: Helps create synthetic dusty solar-panel scenes.
UAE Desert Sand Particle Dataset
Link: https://data.mendeley.com/datasets/3f9hwr9z6p

License: CC BY
Why: Useful for simulating optical scattering on panels.

6. Battery & Power Management
6.1 Battery Degradation
NASA Battery Dataset
Link: https://ti.arc.nasa.gov/tech/dash/groups/pcoe/prognostic-data-repository/
License: Public
Why: Train models for predicting robot return-to-dock needs.
Oxford Battery Degradation Dataset
Link: https://ora.ox.ac.uk/objects/uuid:f9e2033b-3f4c-4daf-8454-3bfffb6666ae
Why: Robust cycle-life modeling.

7. Mechanical Component / Brush Wear
7.1 Industrial Equipment Wear Datasets
NASA Bearing & Motor Fault Dataset (IMS)
Link: https://www.nasa.gov/content/prognostics-center-data-repository
Why: Predictive maintenance proxy for brush-wear patterns.
CWRU Bearing Dataset
Link: https://engineering.case.edu/bearingdatacenter
Why: Vibration analysis → useful for brush vibration wear detection.

8. Docking & Fiducial Marker Datasets
8.1 Fiducial Marker Navigation
AprilTag Dataset
Link: https://april.eecs.umich.edu/software/apriltag.html

License: BSD
Why: Easy markers for precision docking alignment.
ArUco Dataset
Link: https://www.uco.es/investiga/grupos/ava/node/26

License: BSD
Why: Visual docking for solar farms.
III. RECOMMENDED MISSING DATASETS TO CREATE
These datasets do not exist publicly but are critical:
Dust Accumulation Sequence Dataset
Daily images of solar panels over weeks
Annotated dust thickness (g/m²)
Correlated energy drop
Robot Brush-Interaction Dataset
Brush rotation torque
Vibration signatures
Residue removal effectiveness
Brush-wear observations
Solar Panel Edge Geometry Dataset
Close-up high-res images of panel frames
For edge-following navigation
Docking Station Visual Dataset
RGB-D views under different lighting
Night IR docking images
High-Resolution Thermal + RGB Paired Dataset
Thermal vs dust correlation maps

IV. SYNTHETIC DATA GENERATION PIPELINE

A complete synthetic dataset strategy using Blender, Unreal Engine, or Isaac Sim:
Step 1: 3D Models
Import CAD models of solar panels
Add dust particles using particle systems
Simulate sand dune deposition

Step 2: Lighting Variation
Simulate:
midday sun
dawn/dusk
cloudy
hazy/dust storm conditions
reflective glare

Step 3: Dust Simulation
Vary particle size, coverage, streaks, patchiness
Add lens dust to simulate camera degradation

Step 4: Thermal Simulation
Assign emissivity values
Simulate heat retention in dusty vs. clean areas

Step 5: Robot Simulation
Full Gazebo or Isaac Sim environment
Capture multimodal:
RGB
Depth
IR
LiDAR
IMU

Step 6: Annotation Generation
Automatic masks for:
dust regions
panel boundaries
obstacles
docking markers

V. EVALUATION METRICS FOR DATASET QUALITY
1. Image Quality
Resolution (≥1080p recommended)
Sharpness (LAPV)
Signal-to-noise ratio

2. Annotation Quality
IoU for segmentation masks
Pixel accuracy
Inter-annotator agreement (Cohen’s Kappa)

3. Dataset Diversity
Dust coverage variation
Lighting diversity
Panel angle diversity
Environmental variation (sand, dust, pollution)

4. Representativeness
Correlation with real-world conditions
Panel type diversity (mono, poly, thin-film)

5. Time-Series Dataset Quality
Missing data rate
Sampling frequency

Seasonal coverage

Multimodal correlation (energy + weather + dust)
