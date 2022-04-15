# SLAM-Literature

ORB-SLAM:	a	Versatile	and	Accurate Monocular	SLAM	System:

In	this paper, a	discussion	on	the	previous state	of	art,	its	limitations	and	the	areas	of	improvement	for
implementations of	monocular SLAM	is	presented. A	new	holistic approach is	taken	to	improve	upon	the	existing	
PTAM	method	for	mapping	and	localization	of	a	monocular	camera,	by	implementing	techniques	such	as	real-time	
ORB	based	feature	extraction,	pose-graph	loop	closure,	bundle	adjustment and Levenberg-Marquardt optimization
algorithms.	This	is	followed	by	extensive	experimental	validation	in	order	to	determine	the	accuracy	of	the	system	
for	process	sequences	from	indoor	and	outdoor	scenes	to	hand-held	and	robot	motion.



Visual-lidar	Odometry	and	Mapping:	Low-drift,	Robust,	and	Fast:

In	this paper, an	overview	of an	online lidar-based	visual	odometry technique	is	provided.	The	method described
primarily	tackles	errors arising	from	aggressive	motion	and	temporary	lack	of	visual	features.	The use	of visual	
odometry	is	primarily	for depth	map	creation at high	frequencies (rapid	motion), while	lidar	odometry permits	the	
use	of	point	clouds to	accurately	map	the	environment and	refine motion estimation. Validation	is	performed	with	
the	experimental camera-lidar	setups and	configured	KITTI	datasets to	test	both	the	accuracy	of	mapping	and	
estimation,	as	well	as	robustness	of	the	system	during	rapid	motions and	lighting	changes.



Dense	Tracking	and Mapping in	Real	Time:

This paper presents a	superior	alternative	to	Monocular SLAM	using dense	3D	surface	modelling and	whole-image	registration-based	
camera	tracking over	static	scenes.	The	3D	surface	modelling	is	achieved	from	multi-view	stereo	reconstruction	of	depth	maps	from	various	
frames. The	tracking	problem	is	solved	by	dense	whole	image	alignment	at	a	specified	frame-rate,	while	the	mapping	problem is	resolved by	
accumulating	depth	maps	from	multiple	images in	a	cost	volume	and	is	then	optimized and	regularized	to	extract	depth	data using a nonconvex	framework. The	system	demonstrates	impressive	real-time	performance	for	un-ideal	conditions,	and	results	appear	to outperform	
strong	classic algorithms.	



DeepTAM:	Deep	Tracking	and Mapping:

This paper presents a	deep	learning	approach	to	SLAM	as	an	improved	alternative	to	Dense	Tracking	&	Mapping.	Here, a system	for camerapose tracking and	depth	map	estimation is	designed	to	reduce	common	biases in	camera	motion	by	considering	many state	hypotheses and	
an	image-prior-based refinement	approach. The	tracking	problem	is	reduced	to	estimating	a	small	pose	increment	‘δT’ between	a	virtual	
frame	and	the	current	frame, reducing motion	noise,	while	the	mapping	problem is	resolved	by	accumulating	depth	maps	from	multiple	
images in	a	cost	volume	and	is	then	optimized and	regularized	to	extract	depth	data. The	system	is	trained	extensively	using	Adam	and	
Tensorflow,	and	results	appear	to outperform	strong	classic	and	deep	learning	algorithms.	



KinectFusion:	Real-Time	Dense	Surface	Mapping	and	Tracking:

In	this paper, the objective	is	to	achieve	an	accurate	real-time	SLAM	system	by	creating	a	global model	from	depth	data	from	a	Kinect
sensor	for	an	observed	scene. Dense	vector	maps	and	pyramid	mapping	techniques are	employed	to	extract	data	from	the	Kinect
sensor.	A	scene	model	3D	reconstruction	is	achieved	with	a	specific volumetric and	truncated signed	function, which is	combined	
with	the	pose	information and	ray-casted	into	an	estimated	frame,	yielding	a	so-called dense	surface	prediction	against which	the	
actual	depth	map	from	the	current	pose	is	aligned.	In	order	to	accurately	estimate	the	sensor-pose,	an	ICP	alignment	between	the	
surface	prediction and	current	sensor	data is	applied
