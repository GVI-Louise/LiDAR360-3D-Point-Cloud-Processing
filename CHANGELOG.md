LiDAR360 Version Release Notes
============================
v8.0 - 8/15/2024
----------------------
- **Preprocessing**：
	* Add 3D Control Point Report:
	 - Add automatically targets detection and control points matching.
	 - Add direct definition of transformation models in control point reports.
	* Add DJI L1 / L2 Reconstruction, supporting UAV Processing workflow.
	* Optimize Trajectory Adjustment, supporting massive point cloud and image combined adjustment, target detection from point cloud / image and matching control point to improve data precision.
	* Optimize Data Registration:
	 - Add Define UCS to change point cloud coordinate by local cartesian coordinates.
	 - Add support for importing control points as reference data option for point pairs registration.

- **Data Management**：
	* Add Adjust Point Cloud Color.
	* Add Unit Conversion, supporting all platform format.
	* Add Convert ASCII to Vector / Convert Vector to ASCII.
	* Add support for defining projection / reprojecting for raster, vector and ascii file.
	* Add support for selecting target coordinate from layers.
	* Add Convert LiTIN / LiModel to OBJ / OSGB.
	* Add 3D affine parameters in Transformation Calculation.
	* Optimize Normalization to mitigate object cracking caused by steep slope.
	* Optimize Segment by Attribute, supporting using additional attributes for statistic.
	* Optimize Convert to TIFF, supporting fixing holes.
	* Optimize Raster Subdivision, supporting generating tile boundary line.
	* Optimize Extract by Return, supporting 1~15 return number.

- **Classification**：
	* Add support for road classification and outline extraction.
	* Add support for classify roof and wall in Classify Buildings.
	* Optimize Classify by Deep Learning, supporting new Scenes.
	* Optimize Classify Ground Points, supporting Concurrency processing.
	* Optimize Classify by Custom Deep Learning:
	 - Add support for set trained model as a new function.
	 - Add support for image labeling, training and inferencing.
	 - Add Classify Tunnel by deep learning trained model.
	 - Optimize point cloud deep learning model.
	* Optimize Classification Editor:
	 - Add automatically saving setting.
	 - Add semi-auto classify by SAM.
	 - Add seed point selection for classify by select area operation.
	 - Optimize Simulate Ground Points tool, supporting random distribution.
	 - Optimize memory usage.
- **Forestry**：
	* Add Forests Stands Delineating.
	* Add built-in tree model library for Generate Tree Model, supporting 70 Tree Species.
	* Optimize Individual Tree Attributes Calculation:
	 - Add support for trunk curvature calculation.
	 - Add support for trunk section and trunk volume calculation.
	 - Add support for forked DBH extraction and management.
	 - Optimize tree height and DBH calculation.
	 - Optimize forestry setting option, supporting individual tree attributes setting.
	 - Optimize forestry setting option, supporting individual tree attributes setting.
	* Add Stand Analysis and report, supporting Thinning Analysis and Standing Tree Volume Analysis.
	* Add View Azimuth and Distance.
	* Add support for exporting individual tree attributes as table / vector file.
	* Add support for point cloud display by tree attributes by treedb linked.
	* Add CHM Pits Filling to fix holes in coniferous forests CHM.
	* Optimize Individual Tree Report, adding tree number, area information, pano image and supporting pdf format.
	* Optimize Regression Analysis, adding scatter plot result.
	* Optimize Trunk Based Segmentation to improve result accuracy.
	* Optimize Extract by Tree ID , supporting extract individual tree to LiData / Las format.
- **Terrain**：
	*  Add REM.
	*  Add Flood Analysis.
	*  Add View Analysis.
	*  Add Sky View Factor.
	*  Add Annual Insolation.
	*  Add Solar Radiation.
	*  Optimize LiTIN / LiModel Editor, supporting undo and redo operation for each step.
	*  Optimize LiModel Editor, supporting adding various breaklines.
	*  Optimize Contour Editor, supporting topology checking and select area filtering.
	*  Optimize DOM, supporting color correction.
	*  Optimize generate contour functions, supporting more simplify and smooth methods.
	*  Optimize DEM, supporting add point cloud name to results in standard model, expanding scale to 1:5000.
	*  Optimize Section Analysis, supporting quality inspection and more analysis result.
	*  Optimize Generate Elevation Annotation, supporting diamond sampling.
	*  Optimize Change Detection, supporting missing data area annotating.
- **Mine**：
	* Add Extract Tunnel Centerline.
	* Add various section analysis results for tunnel.
- **Building**：
	* Add support for attributes editor in Building Editor.
	* Add support for building attributes calculation, extension, filtering and so on.
	* Optimize building attributes calculation, supporting calculating rmse between point cloud and model.
	* Optimize operation of Matched Photos Editor.
	* Optimize LiBIM file rendering to reduce lag when handling laege data.
- **New Photo Module**
	* Add New Project, support for infrared and multispectral data.
	* Add Align for aerial triangulation processing, support GPU acceleration.
	* Add Filter Tie Points, supporting automatic / semi-atuo selection.
	* Add DOM Editor.
	* Add Ground Control Points, supporting control points picking and automatic detection.
	* Add Camera Calibration.
	* Add Undistort.
	* Add Defogging.
	* Add support for image project tie points rendering, supporting display by projection error and so on.
	* Optimize Align to Point Cloud, supporting improve accuracy by camera calibration, control points picking and automatic detection.
- **New Distributed Module**
	* Add various functions for distributed computing.
	* Add support for large data and multiple data sets.
	* Add support for dynamic configuration of compute node priorities.
	* Add support for multi-instance computation, monitoring, and management of compute nodes.
	* Add support for merging results.
- **Vector**
	* Add Extract Feature by SAM.
	* Add Trace Toe Tool.
	* Add Attach to Ground.
	* Add Respace Geometry.
	* Add Orthographic Draw Line.
	* Add Round Corners.
	* Add Trim Polyline.
	* Add Convert to Polyline / Polygon.
	* Add support for exporting label me format for image deep learning.
	* Optimize and merge some tools.
	* Optimize drawing curve tools, supporting set parameters to generate curve.
	* Optimize vector layer management, supporting layers modify setting.
	* Optimize Copy Parallel, supporting copy distance setting.
	* Optimize vector setting, supporting symbology and snapping setting.
	* Optimize vector editor operation, adding operation prompts.
- **Other**
	* Add unit setting, supporting processing and generating result in different unit.
	* Add Share Data in LiCloud, supporting viewing and sharing data online.
	* Add measurement setting, supporting snapping different data type to improve measurement accuracy.
	* Add Line Above / Below, Plane Above / Below / Inside Selection.
	* Optimize Volume Measurement and report, supporting point cloud image, adding basic information and image setting.
	* Optimize Profile View, supporting setting linked viewer setting.
	* Optimize vector file display, supporting show or hide control by layer.
	* Optimize project directory tree:
	 - Add image project display control, supporting adjusting image size, exporting and so on.
	 - Optimize table / vector(shp / gpkg) / LiBIM attributes table management, supporting attributes calculation.
	 - Optimize table file display, supporting dynamic adjusting label size and so on.
	* Optimize option setting, supporting cpu selection, unit settings, more forestry settings.
	* Optimize Batch Processing, supporting more functions.


v7.0 - 6/10/2022
----------------------

- **Preprocessing**:
	* Add mirror angle correction in trajectory adjustment for livox laser
	* Add hybrid adjustment, improve point cloud accuracy
	* Optimization data registration process, supports registration of point clouds and models
	* Add auto split trajectory for boresight
	* Add Z-value recording in projection coordinates when trajectory solving

- **Data Management**:
    * Add point cloud color brightness  and contrast control tool
    * Add smoothing line tool, provide multiple smoothing methods
    * Add batch point clouds to PLY tool
    * Add building model export to DAE
    * Add smoothing meshes tool

- **Classification**:
    * Add deep learning urban/Rural scene classification
    * Support multiple segment classification for classify by height above ground

- **Terrain**:
    * Add construction progress analysis tool
    * Add contour consistency check tool
    * Add generate elevation annotation points on contour lines
    * Support external aerial projects for generate DOM
    * Optimize TIN to DEM tool to solve the problem of external interpolation outside boundary
    * Optimize dimming of mountain shadows
    * Section analysis
     - Support tunnel section parameterized design
     - Support generating section based on slope
     - Support distance display for section comparison

- **Forestry**:
    * Add biomass estimation and biomass model management
    * Add deep learning-based individual tree segmentation to improve tree detection
    * Add forestry attribute custom format to simplify attribute usage
    * CHM segmentation adds east-west and north-south crown width parameter extraction

- **Mine**:
    * Add inter-ramp compliance tool
    * Optimize toes and crests extraction, support auto-separating of toes and crests
    * Add mesh editor tools, allow automatic and semi-automatic fill holes, hide selection, model decimate, and smooth tools
    * Optimize mesh surface reconstruction to improve speed and effectiveness
    * Mesh editor
     - Support both front and back mesh display, and overlay display of points, lines, and surfaces
     - Support mesh selection tools such as lasso, polygon, and rectangle
     - Support mesh back faces selection and invert selection
     - Support mesh visible and through selection
     - Support selection expand and shrink, component selection, and flood selection
     - Support hide selection, select all, and unselect all
     - Support filling all holes and filling single holes
     - Support bridge tool
     - Support mesh smooth
     - Support mesh decimate

- **3D Building**:
    * Add extracting building footprint from image
    * Add building model registration with image
    * Add projecting textures from photos
    * Add manual image texture mapping, material texture mapping, and material library management
    * Add building attribute management, including adding, deleting, and editing attributes
    * Add attributes calculate, including volume, height, and house shape
    * Improve building model editing
     - Add split building
     - Add fit patch
     - Add extrude building
     - Building split supports  polyline segmentation
     - Add file management after deletion

- **UAV Processing**:
   * Supports one-click processing of trajectory adjustment, pos process, cut point cloud by trajectory, cut overlap, smooth points, subsampling, remove outliers, classify ground points, classify by deeep learning

- **Vector Editor**:
   * Add merge polygon
   * Support gpkg data format
   * Add vector text labeling
   * Add intersect polylines
   * Add copy parallel
   * Add extract building footprint from Mesh
   * Supports large data LOD drawing, improving editing efficiency
   * Support show vertices settings

- **Platform**:
   * Add vector display line width setting
   * The directory tree adds trajectory and imageproject management
   * Support selection of attribute fields to display, data saving as new, attribute editing, and attribute filtering
   * The selection and clipping tool supports saving remaining data
   * Volume measurement reporting support and saving the current scene graph
   * The rolling screen tool supports multiple data types such as point clouds, models, vectors, and tables
   * Mesh editing, LiBIM, LiModel, LiTIN, and other editing supports shortcut key settings
   * Support gradient background color setting for rendering scene

v6.0 - 8/10/2022
----------------------

- **New Modules and Features**:
	* Added voxel down-sampling when loading data is converted to LiData
	* Added strip adjustment function for multiple sorties
	* Added conversion based elevation projector plane coordinate
	* Added support for KML vector format
	* Vector Drawing
	    - Added arc drawing
	    - Added the drawing of one point circle, two point circle and three point circle
	* Added building modeling module
	    - Added automatic building of LOD2 level model based on base map
	    - Added semi-automatic building of LOD2 level model
	    - Added building model editing tool
	     * Added vertex moving tool
	     * Added vertex deleting tool
	     * Added vertex adding tool
	     * Added line removal tool
	     * Added line alignment tool
	    - Added building model plane editing tool
	     * Added sheet merge tool
	     * Added sheet removal tool
	     * Added the face intersection line tool
	     * Added the tool for add faces
	    - Added building ground elevation adjustment
	    - Support the output of building models in obj, fbx, cityjson, and other formats
	    - Support LiBuilding data consolidation
	* Forestry module
	    - Added individual tree segmentation and matching tools
	    - Added tree 3D modeling
	    - Added export of individual tree report
	    - Added tree trunk extraction tool based on TLS data
	    - Added tool for extracting crown base height of individual tree
	    - Added TLS porosity calculation
	    - Added TLS cover degree calculation
	    - Added TLS individual tree editor
	     * Added semi-automatic support removal tool
	     * Added individual tree attribute filter check
	    - Added airborne forestry individual tree point cloud editing tool
	     * Added semi-automatic individual tree point cloud segmentation
	     * Added attribute-based filter check
	     * Added the operations for creating, deleting, and merging individual tree point cloud
	* Terrain module
	    - Added DOM production tool based on DEM\DSM
	* Added Custom Deep Learning Classification Tools
	    - Support customized process for training and reasoning tasks
	    - Support model management
	    - Support algorithm update
- **Enhancements**:
	* Shortcut keys are supported for clipping tool selection
	* Point cloud fitting plane can be used as the measurement datum for volume measurement
	* Split window rendering mode is supported for point cloud rendering
	* The efficiency of point cloud conversion to LiData data is improved by 30%
	* The efficiency of common tools such as smoothing, denoising and resampling are optimized, and the parallel mode is improved by 50%-120%
	* Model data architectural semantic rendering is supported
	* Project Management Window
	    - Import of *.ligeo and *.mmprj project data is supported
	* Clipping tools
	    - “Tile by polygon” supports buffer settings
	    - Single point drawing of rectangular areas is supported for rectangular clipping
	* Control of object move tool is supported for manual translation and rotation
	* Classification
	    - The classification of tower and power line is expanded through deep learning of relevant classification
	* Terrain
	    - Whether the section is controlled by interpolation is supported for road section analysis tool
 
v5.4 - 07/25/2022
----------------------

- **New Modules and Features**:
	* Added the function of extracting by additional attributes
	* Added the function of segment by attribute
	* Volume Measurement
	    - Added the triangulation method for volume measurement for more accurate calculation
	    - Added volume measurement of solid model
	* Projection and coordinate conversion
	    - Added geoid option
	    - Support independent selection of horizontal projection and vertical projection
	    - Added four parameters and geoid joint conversion
	    - Added geoid surface model fitting
	    - Added model data conversion options to the manual rotation and translation and the manual registration tools
	* Added the function of classification by additional attributes
	* Added model smoothing function
	* Vector Editing
	    - Added point break, line break, merge, delete functions
	    - Added Bspline and BezierSpline drawing
	    - Added Bspline and BezierSpline shaping
	    - Added 2D and 3D vector drawing elevation mode settings
	    - Added polyline smoothing tool
	    - Added highest and lowest points snapping
	* Added the function of manual tree species marker
	* Added individual tree attribute settings and the support of selection of calculation methods such as tree position and crown width
	* Vector editing
	    - Support extracting toes and crests
	    - Support volume change analysis
- **Enhancements**:
	* Added gallery mode to the common editing tools in the interface, which supports floating display of tools
	* The classification class supports 0-255 class selection
	* Support 2D and 3D data linkage
	* Custom tab settings window supports tool searching
	* Data rendering
	    - Added raster, vector, model, and table data to display by window
	    - Display by window supports point cloud, raster, vector, model, table data filtering by value range
	    - Added raster data hillshade feature rendering
	    - Support data to save the last right-click attribute rendering settings
	* Multi-point selection supports coordinate positioning
	* Strip alignment supports the use of selected categories for boresight error calculation
	* Trajectory adjustment supports the import of multiple trajectories
	* Control point report supports import label display and export report format setting
	* Point cloud subdivision functions support preview
	* Boundary extraction supports extraction to the same vector file
	* Classification editing
	    - Added the semi-automatic classification of buildings and noise points
	    - Support 3D editing mode
	    - Support joint image editing
	    - Support block editing by range, scale and external import range
	    - Improved the function of ground point simulation
	* TLS seed point editing
	    - Support profile and main window position displaying
	    - Added shortcut keys for the main window height filter function
	    - Profile view window supports range line display
	    - Optimized DBH batch extraction function to improve tree recognition accuracy
	* Clear TreeID tool supports height filtering 
	* Optimized the display of geostatistical rose diagram
v5.3 - 03/20/2022
----------------------

- **New Modules and Features**:
	* Added building and vegetation categories based on deep learning
	* Added DEM Edge Alignment
	* Added DEM accuracy assessment
	* Added CSF filter
- **Enhancements**:
	* Section Viewing and Editing
	    - Added vertical stretch display
	* Section classification editing
	    - Added ground point simulation
	    - Added DEM preview
	    - Support frame selection of multiple blocks to construct and edit block data
	* Color rendering
	    - Added real-time contour rendering
	    - Improved the convenience of rendering point cloud attributes
	* Ground point classification supports terrain scene selection
	* Support coordinate and projection transformation during point cloud data import
	* Manual translation and rotation tools support setting the rotation center
	* Improved the efficiency of generating contour lines by 2-10 times
	* Optimized the efficiency of functions such as denoising, smoothing, ground point classification, noise filtering, etc. Support multi-threading and memory resource settings in the options
	* Optimized the image rendering operation experience and improve the fluency
	* Solved the problem of shortcut keys customization conflict, support unified control

v5.2 - 11/19/2021
----------------------

- **New Modules and Features**:
	* Breakline
		- Point cloud profile editor supports breakline drawing
		- Improved LiTIN editor breakline drawing
		- Support adding breaklines to DEM
		- Support adding breaklines to contour lines
	* Added extract water area tool
	* Support point clouds in PCD format
- **Enhancements**:
	* Section
		- Support create section by adding model data
		- Support adding section at any position
		- Optimized create section by point cloud and fix the missing section caused by the missing point cloud
		- Optimized export of section to meet production requirements
	* Optimized Projection and Coordinate Conversion, add support for storage of user-defined conversion models, parameters can be created and applied directly
	* The measurement tool supports unit setting
	* Optimized the efficiency of the control point report function with an average increase of 40%
	* Generated CHM function to support big data processing
	* Strip alignment supports SBET format trajectory data
	* Contour function supports class selection
	* Roaming tool supports pause during roaming
	* Added trial application on start page
	* Point cloud data GPS time conversion supports selecting date for conversion
	* Mutual conversion between shp and kml supports geographic coordinate system
	* Subdivision tool supports buffer setting
	* Support report custom settings
	* Optimized the bit rate of the screen recording tool to provide a default value based on the system resolution

v5.1 - 07/29/2021
----------------------

- **New Modules and Features**:

	* Added mine module
		- Extract tunnel points
		- Compute normal vectors
		- Triangulation modeling
		- Poisson modeling
	* Vector editing
		- Support 3D vector drawing
		- Added tools for shaping elements
		- Added split polygon tool
		- Added semi-automatic extraction of building outlines
		- Added semi-automatic extraction of road shoulders
		- Added intersection drawing line
		- Added section auxiliary drawing
		- Added associated window to assist drawing
		- Added selection file editing
		- Added temporary draft editing
		- Support 3D capture
		- Support 3D selection
		- Support shortcut keys setting
		- Support rollback and redo
	* Added the hover mode, support the use of hover mode under measurement point selection
	* Added cutting by straight line
	* Added dividing by polygon
- **Enhancements**:
	* Profile editing and classifying
		- "Select tool" supports category settings to be individually set and recorded 
	* "Select cutting" supports cutting of the triangulation model
	* Individual tree point cloud editing supports directory tree control display and hidden
	* "Cut by polygon" supports inner and outer cutting options
	* Manual translation and rotation support XIYZ component progress control
	* Directory tree
		-	Support right-click to open the folder
		-	Vector data supports dxf format

v5.0 - 01/29/2021
----------------------

- **New Modules and Features**:

	* Added geology module
		- Added flow direction function
		- Added flow direction function cumulant
		- Added fill function
		- Added slope/aspect query function
	* Added data IO API for software development
		- Support creating LiData point cloud file
		- Support reading LiData point cloud file
		- Support modifying LiData point cloud file
	* Added powerline module
		- Added deep learning of powerline classification
		- Added danger point detection function
		- Added customization of the danger point detection
		- Support danger point visualization
	* Added point cloud smoothing function
	* Added trunk extraction function
	* Added elevation annotation points generation based on contour lines function
 	* Added new format transform tools
		- shp to kml
		- kml to shp
	* Support background grid display in viewers
	* Support extracting point cloud by TreeID
	* Support clear individual tree record and segmentation by TreeID
	* Added calculation of forest metrics
- **Enhancements**:
	* UI
		- Brand new Ribbon user interface style
		- Support free dragging of child windows
		- Support customization of UI pages
		- Support automatic hiding of docked window
		- Support one-click industry application processing
	* Strip alignment
		- Added strip adjustment function
		- Support clipping trajectory by the quality and selecting with a brush on a trajectory
	* Directory tree
		- More comprehensive point cloud information display
		- Support selecting the version of the LAS file when right-clicking to export
		- Support right-clicking to add additional attributes of point cloud
		- Support right-clicking to rename files
		- Support setting the point size of table data
	* Expanded the projection library to support more projections and geoid surface
	* Optimized PCV efficiency to support more point cloud calculations for PCV
	* Optimized ALS automatic individual tree segmentation
	* Improved point cloud attribute expansion of an individual tree to support slope and altitude information
	* Optimized individual tree seed point editing
		- Improved method of profile selecting
		- Improved method of adding and deleting seed points
		- Added viewpoint position and direction for easy positioning of trees
		- Real-time update of attribute table corresponding to seed point modification
		- Support undo and redo
		- Support setting profile viewpoint distance
	* Optimized individual tree point cloud editing
		- Improved method of profile selecting
		- Support creating an individual tree by specifying a chosen tree
		- Support setting profile viewpoint distance
		- Automatic saving of configuration
	* Optimized profile point cloud editing
		- Improved the efficiency of block editing by more than 50%
		- Support mouse position tracking in the profile window
		- Support data exporting
	* Added section comparing analysis function in section analysis
	* Upgraded LiModel format to solve the problem of coordinate accuracy loss
	* Reduced the GPU usage rate of point cloud display by 20%
	* Support multiple calls to the same function in batch processing
	* Fixed the bug when using cross selection and clipping tool simultaneously
	* Improved the efficiency of point cloud conversion to DXF file
	
v4.1 - 06/08/2020
----------------------

- **New Features**:

	* Added three-point angle measurement
	* Added registration of UAV and backpack forestry point cloud data
	* Added individual tree attribute information expansion
	* Added detection of forest structure changes
	* Added DBH measurement
	* Help menu
		- Added software usage problems and demand feedback channel
		- Added FAQ, quick start, official website link, etc.

- **Enhancements**:

	* Optimized the efficiency of loading multiple files
	* Improved color rendering of point cloud attributes
	* Additional attribute management
		- Support deleting
		- Support component combination rendering
	* Improved profile editing and classifying
		* Support grid scale display in profile window
		* Support directory tree to manage point cloud tiles in memory
	* Support import boundary of measurement area with SHP file in volume measurement
	* Improved the efficiency of filtering function and the density of ground points
	* Support directory tree to manage point cloud tiles in memory in individual tree point cloud editing function
	* Support combined calculation in forestry metrics
	* Support extract point cloud by tree ID, support export the extracted point cloud to LAS and LiData format
	* Support attribute filtering in ALS seed point editing
	* Improved LiTIN editing, support 3D view editing, and support the setting of starting height of broken line
	* Added tunnel cross-section in cross-section analysis
	* Window layout supports multiple layout modes
	* Newly designed UI icons

v4.0 - 12/30/2019
----------------------

- **New Features**:

	* Added denormalization tool
	* Added classifying close points tool
	* Added manual rotation and translation tool
	* Added convert ASCII to BLH tool
	* Added individual tree editor tool. Support to create, merge, and delete tree
	* Added statistics individual tree attributes tool
	* Added TLS leaf area index tool
	* Added ALS forestry metrics calculation in give area tools
	* Added deviation analysis tool for two data of the same area collected in different times
	* Added change detection tool
	* Added GPS time transformation tool which supports transforming GPS time between GPS coordinated time and GPS week and second

- **Enhancements**:

	* Support online update checking and installing
	* Upgraded the version of LiData to V2.0 which supports all the features of Las1 .4 (except the waveform information) and the additional attribute of the point cloud file
	* Support the color rendering for all the attributes of point cloud data
	* Support the rotation of 2D view
	* Support fast mode and precise mode in volume calculation and providing the information of the measuring area
	* Support zooming to the layer by double-clicking the file in the directory tree
	* Support recovering the data association in the same path for the project file path
	* Support EDL effect in render to file and save to video tools
	* Support generating automatic alignment report and clearing the data alignment information
	* Improved the profile editor which supports customizing shortcut keys and solves the problem of profile buffer settings
	* Improved the EDL effects in orthogonal projection
	* Improved the cross selection tool which supports data clipping when being used with selection tool, or 2D drawing when being used with Vector Editing.
	* Improved data interaction experience:
		- Improved browsing fluency
		- Support automatically picking the rotation center
		- Improved point picking experience
		- Support measuring components in the measurement tools
		- Support measuring points number in the density measurement tool	
	* Support recording the original Z value in normalization tool
	* Improved the data formats supported:
		- Support E57 point cloud format
		- Support additional attributes for LAS, PLY, and ASCII format point cloud files
		- Support choosing the version of las file when exporting point cloud in las format (las 1.2, las 1.3, and las 1.4)
		- Support converting version of LiData (V 1.9)
		- Support converting point cloud in Geographic Coordinate System to projected LiData
	* Improved the calculation method of individual tree crown volume
	* Improved the efficiency of the calculation of forestry metrics

v3.2 - 06/06/2019
----------------------

- **New Features**:

	* Added brightness settings tool
	* Added ICP registration function
	* Support exporting TIN in DXF format
	* Added raster statistics tool 
	
- **Enhancements**:	

	* Optimized EDL display effect in profile editing mode
	* Optimized the ground point filter
	* Optimized the efficiency and effect of "Classify Buildings" tool
	* Support rectangular/circular interactive area selection tool in clipping function
	* Changed band calculator to raster calculator which supports custom formula
	* Shortcut keys and right-clicking menu in ALS individual tree segmentation editing tool
	* Support position uncertainty optimization mode in regression analysis
	* Support corresponding multiple point cloud files to one trajectory in "cut point cloud based on trajectory" tool
	* Profile editing and classifying: 
		- Added the lasso selection tool
		- Added the plane detection tool
		- Support clearing the triangular network already been built
		- Support setting the size of brush selection tool
		- Support setting the step length of the profile translation
		- Optimized the efficiency of triangular network generating
	* TLS individual tree segmentation editing:
		- Support ignoring the Z-values of the input seed file
		- Support right-clicking menu and shortcut keys
		- Support hot keys in single tree attributes measuring
		- Support display of LiBackpack trajectory file
	* Manual registration:
		- Support inputting/outputting coordinate transformation matrix
		- Support the preview of transformation
	* Raster and table data:
		- Support color settings
		- Support highlighting objects when they are selected
		- Support centralizing the objects when they are double-clicked

- **Bug Fixed**:

	* Fixed the bug that the order of the vector and table data's attribute table is wrong
	* Fixed the bug that only the displayed data will be used in "batch extraction DBH" tool
	* Fixed the bug that profile selection will disappear in the main window if users edit point cloud in profile window

v3.1 - 12/31/2018
----------------------

- **New Features**:

	* Profile editing and classifying:
		- Support block editing and classifying
		- Support multiple windows selecting and classifying
		- Add the brush selecting tool
		- Block editing mode supports to undo/redo
		- Added the automatic timing/automatic saving function
		- Added multiple selecting area filter classification/classification setting tools
		- Support shortcut keys switch function
		- Block editing mode supports RAM usage warning

	* Added convex hull and concave hull mode for boundary extraction
	* Added check for updates function

- **Enhancements**:	

	* Improved the efficiency of LiData generating
	* Support to recalculate the histogram of point cloud intensity and elevation
	* Moved the rectify to reprojection and conversion module
	* Multiple point selecting tool supports to customize the extended attributes
	* Support projected coordinate systems in JGD2011 coordinate system
	* Support POS files in more formats. Now support POS file with projected coordinates
	* Support converting length units for las and LiData files


v3.0.1 - 12/10/2018
----------------------

- **New Features**:

	* TLS individual tree segmentation editing:
		- Added circle selection tool
		- Added profile translation tool
		- Added DBH inspector tool

- **Enhancements**:	

	* Optimized the color rendering for individual tree segmentation.
	* Optimized the segmentation of the vector boundary of crown in CHM individual tree segmentation.
	* Support the .shp file in section tool.

- **Bug Fixed**:

	* Fixed the bugs already known
	
v3.0 - 10/16/2018
----------------------
- **New Features**:

	* Added saving users’ parameters settings as default, and the prompt of the information about each parameter when putting mouse on it
	* Support the spike-free TIN generation algorithm
	* Added the random forest regression model
	* Added the regression predict analyze
	* Added the Projection and Coordinate Conversion Toolset:
		- Seven parameters solution
		- Four parameters solution
		- Vertical datum transformation
	* Added noise classification function
	* Support conversion of raster data to LiData

- **Enhancements**:

	* Improved the ground point filtering algorithm
	* Improved the accuracy and efficiency of the TLS individual tree segmentation tool
	* Upgraded the LiTIN format to support saving the corresponding LiDAR point classes in LiTIN data and display LiTIN data by classes
	* Improved the editing and flattening TIN data in LiTIN format
	* "Tile by range" supports buffer setting and vector exporting
	* Support subdivisions of Graticules
	* Support generating multiple files when performing polygon clipping
	* Support selecting RGB range when convert data to las format

v2.2 - 06/20/2018
----------------------
- **New Features**:

	* Multi-threaded batch processing;
	* Support invoking of command line;
	* Measurement of individual tree attributes (total height, CBH, stem straightness. etc.) from TLS data.
	
- **Enhancements**:
	
	* Improved regression analysis which allows for the importation of independent variables from external sources;
	* Output elevation and intensity variables as .tif formatted files;
	* Individual tree segmentation from a selected point cloud class;
	* Improved TLS data editing tools that allow users to (1) batch process data to extract DBH measurements and (2) fit DBHs to point clouds selected in the profile view window;
	* Added crown diameter, area, and volume to the output of the TLS individual tree segmentation tool;
	* Improved Section Analysis Tool in the Terrain Module now allows users to: (1) analyze .dxf formatted files, (2) import more than one file at a time and draw multiple section lines. (3) define a step value to simplify sections. (4) export multiple section files
	* Output contour feature as 2D polylines;
	* Editing of vector dataset attributes;
	* Improved profile feature user experience. 

- **Bug Fixed**:
	
	* Tree heights now updated for tree filtering after tree segmentation tool has been run;
	* Projection information of las data can now be read.

v2.1.2 - 04/25/2018
----------------------
	
- **Enhancements**:
	
	* Improved batch extraction function for DBH (Diameter at Breast Height);
	* LiData upgrade.

v2.1.1 - 04/08/2018
----------------------
	
- **Enhancements**:
	
	* Support LAZ/LAS 1 .4 file formats;
	* Intensity information with ply data now can be read.

v2.1 - 02/05/2018
----------------------
- **New Features**:

	* Automatic calculation of flight strips matching parameters;
	* Median ground point clouds classification;
	* Supervised classification based on machine learning;
	* Support revising ground point filtering results of a defined region;
	* Support cross section analysis;
	* Vector Editing;
	* Support selected region extends from both end in profile viewer;
	* Tile by Point Number;
	* Support generating TIF images with projection information.
	
- **Enhancements**:
	
	* Improved DEM, DSM interpolation algorithm;
	* Improved efficiency of point cloud and TIN generated contour lines;
	* Improved efficiency of individual tree segmentation algorithm (individual tree segmentation from point cloud and individual tree segmentation based on seed point);
	* Support richer terrain product formats, including a new ASC format for raster data and a new DXF format for the contour line.

- **Bug Fixed**:
	
	* De-redundant function;
	* Multipoint selection;
	* Fixed a bug of Classifying by attribute.

v2.0 - 10/30/2017
----------------------

- **New Features**:

	* New License Key: The software could be activated on a monthly basis or by module;
	* Forest Module (divided to ALS module and TLS module);
		- ALS Module:
			* Seeds generation algorithm: It's used to generate segmentation seed layer based on CHM, Point Cloud Segmentation and Layer Stacking;
			* Seeds edition: adding/deleting seeds, selecting seeds and segmenting individual tree based on seeds;
			* Added individual tree batch processing based on seed layer;
        - TLS Module:
			* Ground Classification using TLS data;
			* Added the seed point based ground point cloud individual tree batch processing;
			* Added the calculation of DBH;
			* Seeds edition: adding/deleting seeds, selecting seeds and segmenting individual tree based on seeds;
	* Classification Module:
		- Improved performance of ground points filter algorithm;
		- Classification for key feature points. By identifying the key surface points, this allows the down-sampling of relatively flat areas thus improving processing efficiency without sacrificing quality;
		- Added a check box to the interface of ground point filter function to extract model key points after separating ground points;
	* Power Line Module:
		- Added creation of vector output for power line and tower classifications;
		- Real-time measurement of the distances from any given point to the closest power line and tower;
	* Added the setting of point cloud display point size for individual layers;
	* Added automatic identification of point cloud center point and setting it as rotation center;
	* Improved visual effects of TIN;
	* Shapefile layer attribute table now can be displayed;
	* Identifying and locating the corresponding individual tree in the viewer by double-clicking a row in the segmentation result list table.
	* Cross selection tool supports more accurate adjustment of the boundingbox;
	* Added Display Parameters Settings in LOG viewer while the LOG file still stays at system's TEMP folder;
	* Support information collection when the software crashes. You can send crash information in the pop up interface to the mailbox;
	* The cut results for multiple data sources can be saved separately or be merged into a file.

v1.5 - 07/14/2017
----------------------

- **New Features**:

	* Added power line module. The main functions include marking tower position, cutting the point cloud data based on the tower position, automatic classification of power line and tower, dangerous points detection and report generation;
	* Added selection toolbar which includes polygon selection, rectangle selection, sphere selection, in cut, out cut, save cut and cancel selection;
	* Added editing point cloud classification with real-time TIN;
	* Support merging multiple files into one;
	* Support undo to profile editing and selection function by Ctrl+Z.
	
- **Enhancements**:
	
	* CHM segmentation algorithm improvement. Users can adjust more parameters and generate the shape file of tree boundary;
	* Added the residual report to the registration function. Users can choose the points for coordinate Conversion;
	* Cross selection result can be export;
	* The parameters setting for batch processing for multiple files and multiple functions can be imported and exported;
	* Improved profile editing efficiency;
	* Users can choose whether to generate minor, basic and major contour when using "point cloud to contour" and "TIN to contour” functions;
	* Added seven parameters transformation for reprojection function;
	* The results of Clip by Circle and Clip by Rectangle can be exported as one file, or saved as individual files according to the extent of circle or rectangle;
	* The real-time coordinates in the status bar are more accurate;
	* Improved user experience of navigating.

v1.4 - 05/31/2017
----------------------

- **New Features**:

	* Added "generate TIN", "TIN edit", "TIN to Contour", "TIN to DEM" functions;
	* Added Grid Volume Statistics function;
	* Added "Camera Roam" and "Save to Video functions”;
	* Fixed the bug of memory leak when loading .ply data.

v1.3 - 04/17/2017
----------------------

- **New Features**:

	* Added PLY data import and export to I/O module;
	* Added elevation difference, overlap and density quality reports to strip adjustment module;
	* Added "Resampling based on octree" and "point cloud convert to DXF" to data management module;
	* Power line classification;
	* Support mix and glass coloring modes in rendering;
	* Batch Processing for multi-files and multi-functions;
	* Geometric correction (support point cloud registration based on points or sphere targets).

- **Enhancements**:
	* Speed improvements for contour generation based on point cloud;
	* Users can set the properties of minor, basic and major contours for "point cloud to contour". The elevation attributes can be read;
	* The boundary of concave polygon is shown for area measurements;
	* The resolution of surface model is not limited to 0.5m.

- **Bug Fixed**:
	
	* Fixed the bug of file opening error when there is an invalid file in multiple .csv files;
	* Fixed the bug of window flash caused by EDL effect in windows 10;
	* Bug fixed for stepwise regression;
	* Bug fixed for software crash caused by opening old version of LiData;
	* Bug fixed where LiDAR360 could not be opened with unstandardized projection settings.

Lite - 02/04/2017
----------------------
Free version, with main functions including data visualization and grid statistics.

v1.1 - 12/22/2016
----------------------

- **New Features**:

	* Software platform update: 2D&3D integration, multiple window linkage, rolling screen, display order changed by drag, cross selection,etc;
	* Strip quality check function;
	* Added generating contour lines based on point cloud;
	* Chinese software version;
	* Bug fixed for raster image subdivision and LiModel with texture.

v1.0 - 10/11/2016
----------------------
First version release of LiDAR360.