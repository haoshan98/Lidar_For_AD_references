# Lidar Point clound processing for Autonomous Driving
A list of references on lidar point cloud processing for autonomous driving
&#x2611;
&#x2612;
## LiDAR Pointcloud Clustering/Semantic Segmentation/Plane extraction 
**Tasks** : Road/Ground extraction, plane extraction, Semantic segmentation, open set instance segmentation, Clustering
* Fast Segmentation of 3D Point Clouds: A Paradigm on LiDAR Data for Autonomous Vehicle Applications ICRA 2017 [[git](https://github.com/VincentCheungM/Run_based_segmentation), [pdf](https://www.researchgate.net/publication/318325507_Fast_Segmentation_of_3D_Point_Clouds_A_Paradigm_on_LiDAR_Data_for_Autonomous_Vehicle_Applications)] &#x2611; [1 | ground segment and non-ground segments clustering]
```
The identification and extraction of ground
points is rather suitable for this application for two main
reasons; (i) they are easily identifiable since they belong to
planes, which are primitive geometrical objects with a simple
mathematical model, and (ii) it is acceptable to assume that
points of the point cloud with the lowest height values are
most likely to belong to the ground surface. This prior
knowledge is used to dictate a set of points for the initiation
of the algorithm and is eliminating the random selection seen
in typical plane-fit techniques such as the RANdom SAmple
Consensus (RANSAC), resulting in much faster convergence.
```
* Time-series LIDAR Data Superimposition for Autonomous Driving [[pdf](http://lab.cntl.kyutech.ac.jp/~nishida/paper/2016/ThBT3.3.pdf)] &#x2612;
* Fast segmentation of 3D point clouds for ground vehicles [[ieee](https://ieeexplore.ieee.org/document/5548059)] [-]
* An Improved RANSAC for 3D Point Cloud Plane Segmentation Based on Normal Distribution Transformation Cells [-]
* Segmentation of Dynamic Objects from Laser Data [[pdf](https://upcommons.upc.edu/bitstream/handle/2117/14119/1259-Segmentation-of-Dynamic-Objects-from-Laser-Data.pdf?sequence=1&isAllowed=y)] &#x2611; [3 | denoising, preprocessing]
* A Fast Ground Segmentation Method for 3D Point Cloud [[pdf](https://koreascience.kr/article/JAKO201720636500852.pdf)] &#x2611; [2 | ground segment only]
* Ground Estimation and Point Cloud Segmentation using SpatioTemporal Conditional Random Field [[pdf](https://hal.inria.fr/hal-01579095/document)] &#x2611; [2 | elevated ground modelling, ground segment only]
* Real-Time Road Segmentation Using LiDAR Data Processing on an FPGA [[pdf](https://arxiv.org/pdf/1711.02757.pdf)] &#x2611; [1 | real time, ground segment only]
* Efficient Online Segmentation for Sparse 3D Laser Scans [[pdf](http://www.ipb.uni-bonn.de/pdfs/bogoslavskyi16pfg.pdf)], [[git](https://github.com/PRBonn/depth_clustering)]  &#x2611; [1 | real time, ground segment only, ready implementation in c++, Velodyne sensor]
* CNN for Very Fast Ground Segmentation in Velodyne LiDAR Data [[pdf](https://arxiv.org/pdf/1709.02128.pdf)]  &#x2611; [2 | real time, ground segment only, Velodyne sensor]
* A Comparative Study of Segmentation and Classification Methods for 3D Point Clouds 2016 Masters Thesis [[pdf](http://publications.lib.chalmers.se/records/fulltext/238602/238602.pdf)] &#x2611; [5 | general reference]
* Fast Multi-pass 3D Point Segmentation Based on a Structured Mesh Graph for Ground Vehicles [pdf](https://ieeexplore.ieee.org/abstract/document/8500552) [video](https://www.youtube.com/watch?v=cwmcuRnWJfE) [-]
* RangeNet++: Fast and Accurate LiDAR Semantic Segmentation [[link](https://github.com/PRBonn/lidar-bonnetal], [[pdf](https://www.ipb.uni-bonn.de/wp-content/papercite-data/pdf/milioto2019iros.pdf)] &#x2611; [1 | novel postprocessing after semantic segmentation, fence]
* Circular Convolutional Neural Networks for Panoramic Images and Laser Data [pdf](https://www.tu-chemnitz.de/etit/proaut/publications/schubert19_IV.pdf)  &#x2611; [2 | car segment only, Velodyne sensor]
* Efficient Convolutions for Real-Time Semantic Segmentation of 3D Point Clouds [[pdf](http://www.cs.toronto.edu/~urtasun/publications/zhang_etal_3dv18.pdf)] &#x2611; [3 | general segment]
* Identifying Unknown Instances for Autonomous Driving/Open-set instance segmentation algorithm [CoRL 2019](https://www.robot-learning.org/) [[pdf](https://arxiv.org/abs/1910.11296)] &#x2611; [1 | open-set instance segmentation]
* RIU-Net: Embarrassingly simple semantic segmentation of3D LiDAR point cloud. [[pdf](https://arxiv.org/abs/1905.08748), [LU-net](https://hal.archives-ouvertes.fr/hal-02269915/document)] &#x2611; [3 | good in cyclist segment]
* SalsaNet: Fast Road and Vehicle Segmentation in LiDAR Point Clouds for Autonomous Driving [[pdf](https://arxiv.org/abs/1909.08291)] &#x2611; [2 | image-pointcloud auto labelling, road and vehicle segmentation]
* SqueezeSegV3: Spatially-Adaptive Convolution for Efficient Point-Cloud Segmentation [[link](https://github.com/chenfengxu714/SqueezeSegV3)] &#x2611; [1 | segmentation, SOTA]
* PolarNet: An Improved Grid Representation for Online LiDAR Point Clouds Semantic Segmentation [[link](https://arxiv.org/abs/2003.14032)] &#x2611; [2 | polar/ring cnn segmentation]
* Scan-based Semantic Segmentation of LiDAR Point Clouds: An Experimental Study IV 2020 [[pdf](https://arxiv.org/abs/2004.11803)] &#x2611; [2 | scan unfolding image-based segmentation]
* Plane Segmentation Based on the Optimal-vector-field in LiDAR Point Clouds [[link](https://ieeexplore.ieee.org/document/9095372)] [-]
* Semantic Segmentation of 3D LiDAR Data in Dynamic Scene Using Semi-supervised Learning [[link](https://arxiv.org/abs/1809.00426)]  &#x2611; [3 | dynamic scene segmentation, Velodyne sensor]
* Learning Hierarchical Semantic Segmentations of LIDAR Data 3DV 2015 [[pdf](https://www.cs.princeton.edu/~funk/3DV15.pdf)] &#x2611; [1 | small object segmentation, pole objects]
* EfficientLPS: Efficient LiDAR Panoptic Segmentation 2021 [pdf](https://arxiv.org/abs/2102.08009), [video](https://www.youtube.com/watch?v=_ay7ci-Nd0E)  &#x2611; [1 | scan unfloding panoptic segmentation, semantic and instance fusion]
* 4D Panoptic LiDAR Segmentation 2021 [[pdf](https://arxiv.org/abs/2102.12472)]  &#x2611; [2 | temporal multi-scan panoptic segmentation]
* urban_road_filter: a real-time LIDAR-based urban road and sidewalk detection algorithm for autonomous vehicles [[git](https://github.com/jkk-research/urban_road_filter), [video](https://www.youtube.com/watch?v=T2qi4pldR-E), [pdf](https://www.mdpi.com/1424-8220/22/1/194/pdf), [code](https://github.com/jkk-research/urban_road_filter)] &#x2611; [1 | real time, road and sidewalk segment, ready implementation in c++]


## Pointcloud Density \& Compression
* DBSCAN : A density-based algorithm for discovering clusters in large spatial databases with noise (1996) [[pdf](https://www.aaai.org/Papers/KDD/1996/KDD96-037.pdf)] &#x2612; 
* Hierarchical Density Estimates for Data Clustering, Visualization, and Outlier Detection [pdf](https://bdpi.usp.br/bitstream/handle/BDPI/51005/2709770.pdf?sequence=1) &#x2612; 
* Building Maps for Autonomous Navigation Using Sparse Visual SLAM Features [[pdf](https://ygling2008.github.io/papers/IROS2017.pdf)] &#x2611; [5 | tetrahedra insertion, deletion and refinement | image input]
```
Feature-based incremental SLAM (pose tracking, local bundle adjustment, loop closure, global optimization), 
real-time 3D dense mapping (dense volumetric representation), and free space extraction (local path planning)
```
* STD: Sparse-to-Dense 3D Object Detector for Point Cloud [pdf](https://arxiv.org/abs/1907.10471) &#x2611; [3 | two stages detection (voxel- and
point-based), detect car, perdestrian and cyclist]
* Fast semantic segmentation of 3d point clounds with strongly varying density [[pdf](https://www.ethz.ch/content/dam/ethz/special-interest/baug/igp/photogrammetry-remote-sensing-dam/documents/pdf/timo-jan-isprs2016.pdf)]  &#x2611; [1 | multi-scale pyramid neighborhood approximation, random forest classifier, terrestrial laser scans]
* The Perfect Match: 3D Point Cloud Matching with Smoothed Densities [[pdf](https://arxiv.org/abs/1811.06879), [code](https://github.com/zgojcic/3DSmoothNet)] &#x2612; [diff angles point cloud matching, siamese network, voxelized smoothed density value (SDV) representation]
* Deep Compression for Dense Point Cloud Maps [[link](https://ieeexplore.ieee.org/document/9354895)] [-]
* Improved Deep Point Cloud Geometry Compression [[pdf](https://hal.archives-ouvertes.fr/hal-02910180/document), [git](https://github.com/mauriceqch/pcc_geo_cnn_v2)] &#x2612; [character data]
* Real-Time Spatio-Temporal LiDAR Point Cloud Compression [[pdf](http://ras.papercept.net/images/temp/IROS/files/1091.pdf)] &#x2611; [5 | stacked frames compression] 

## Registration and Localization
* A Review of Point Cloud Registration Algorithms for Mobile Robotics 2015 [[pdf](https://hal.archives-ouvertes.fr/hal-01178661/document)] [-]
* LOAM: Lidar Odometry and Mapping in Real-time RSS 2014 [[pdf](https://ri.cmu.edu/pub_files/2014/7/Ji_LidarMapping_RSS2014_v8.pdf), [video](https://www.youtube.com/watch?v=8ezyhTAEyHs)] &#x2611; [1 | mixed of two algorithm, real time]
```
-One algorithm performs odometry at a high frequency but low fidelity to estimate velocity
of the lidar. Another algorithm runs at a frequency of an order of
magnitude lower for fine matching and registration of the point
cloud.
-Achieves both low-drift and low-computational complexity without the need 
for high accuracy ranging or inertial measurements.

```
* Fast Planar Surface 3D SLAM Using LIDAR 2016 [[pdf](https://lamor.fer.hr/images/50020776/Lenac2017.pdf)] &#x2611; [2 | register planar surface]
```
-Registering and merge sets of (local) planar surface segments to construct global map
-Preprocess point cloud efficiently by project to three two-dimensional images
-SLAM backend is based on Exactly Sparse Delayed State Filter as a non-iterative way
of updating the pose graph and exploiting sparsity of the SLAM information matrix
```
* Point Clouds Registration with Probabilistic Data Association IROS 2016 [[git](https://github.com/ethz-asl/robust_point_cloud_registration)] &#x2611; [1 | dense-sparse registration, ready c++ implementation]
```
-Aligning a dense point cloud with a sparse one (merge vision-based sensor and laser scanner or two different laser-based sensors)
-Improvement over the standard Iterative Closest Point (ICP) data association policy
```
* Robust LIDAR Localization using Multiresolution Gaussian Mixture Maps for Autonomous Driving IJRR 2017 [[pdf](https://pdfs.semanticscholar.org/7292/1fc6b181cf75790664e482963d982ec9ac48.pdf)], [[Thesis](https://pdfs.semanticscholar.org/a7ce/36bbdf85f1dba6cf16f47ad3799618511960.pdf)]
&#x2612; [local vehicle localization]
* Automatic Merging of Lidar Point-Clouds Using Data from Low-Cost GPS/IMU Systems SPIE 2011 [[pdf](https://digitalcommons.usu.edu/cgi/viewcontent.cgi?article=1081&context=ece_facpub)] &#x2611; [5 | Sphere Outlier Removal (SOR)]
```
-Identifies outliers and inliers to exist ICP algorithm
-By utilizing MEMS (microelectromechanical systems)-based GPS/IMU systems, 
to gather coarse position and pose information at a low cost
```
* Fast and Robust 3D Feature Extraction from Sparse Point Clouds [[pdf](http://jacoposerafin.com/wp-content/uploads/serafin16iros.pdf)] &#x2611; [2 | feature extraction, Velodyne sensor]
```
-3D scan > flat region removal > surface normal computation > segmentation and 3D features extraction > 3D features
```
* 3DFeat-Net: Weakly Supervised Local 3D Features for Point Cloud Registration [[pdf](https://arxiv.org/abs/1807.09413)]  &#x2611; [3 | siamese network]
```
-Achieve weak supervision by utilized GPS/INS tagged 3D point clouds
-Triplet loss for feature alignment
```
* Incremental Segment-Based Localization in 3D Point Clouds [[pdf](https://n.ethz.ch/~cesarc/files/RAL2018_rdube.pdf)] &#x2611; [3 | incremental segment matching]
```
Accumulates the measurements in a dynamic voxel grid, 
then selectively updates the point normals affected by the insertion
```
* OverlapNet: Loop Closing for LiDAR-based SLAM, RSS 2020 [[pdf](OverlapNet: Loop Closing for LiDAR-based SLAM), [git](https://github.com/PRBonn/OverlapNet), [video](https://www.youtube.com/watch?v=96TBjiay59A)] &#x2611; [3 | detect loop closures for range images]
```
-Work with and without odometry information
-Yaw Estimation
```
* CorsNet: 3D Point Cloud Registration by Deep Neural Network, ICRA 2020 [[link](https://ieeexplore.ieee.org/abstract/document/8978671)] [-]
* LPD-Net: 3D Point Cloud Learning for Large-Scale Place Recognition and Environment Analysis ICCV 2019 [[pdf](https://openaccess.thecvf.com/content_ICCV_2019/papers/Liu_LPD-Net_3D_Point_Cloud_Learning_for_Large-Scale_Place_Recognition_and_ICCV_2019_paper.pdf)]  &#x2611; [3 | point cloud based place retrieval, diff  weather and light conditions]
```
-Adaptive local feature extraction module and the graph-based neighborhood aggregation module
-To extract the local structures and reveal the spatial distribution of local features, 
generate global descriptor via end-to-end manner
```
* DH3D: Deep Hierarchical 3D Descriptors for Robust Large-Scale 6DoF Relocalization [[pdf](https://arxiv.org/abs/2007.09217),[project](https://vision.in.tum.de/research/vslam/dh3d), [video](https://www.youtube.com/watch?v=ZxZiwZugG14)] &#x2611; [3 | siamese network]
```
-Learn local descriptor captures multi-level geometric information and channel-wise relations
-Generate the global descriptor by directly aggregating
the learned local descriptors with an effective attention mechanism
```
* Localisation using LiDAR and Camera Localisation in low visibility road conditions Master’s thesis 2017 [[pdf](http://publications.lib.chalmers.se/records/fulltext/250431/250431.pdf)] [-]
* Monocular Camera Localization in 3D LiDAR Maps IROS 2016 [[pdf](http://www.lifelong-navigation.eu/files/caselitz16iros.pdf)] &#x2611; [1 | tracks the pose of monocular camera with respect to a given 3D LiDAR map]
```
-Employ a visual odometry system based on local bundle adjustment
to reconstruct a sparse set of 3D points from image features
-Visual localization advantage: 
only relies on matching geometry, robust to changes in the photometric appearance of the environment
```

## Feature Extraction
* Fast Feature Detection and Stochastic Parameter Estimation of Road Shape using Multiple LIDAR [[pdf](https://www.ri.cmu.edu/pub_files/2008/9/peterson_kevin_2008_1.pdf)] &#x2612; [convolution, Velodyne lidar/radar/laser]
* Finding Planes in LiDAR Point Clouds for Real-Time Registration [[pdf](http://ilab.usc.edu/publications/doc/Grant_etal13iros.pdf)]  &#x2611; [1 | plane detection - side wall, floor, hallway]
* Online detection of planes in 2D lidar [[pdf](https://pdfs.semanticscholar.org/6857/b602dd702664c20febd41dc984451fd97bb3.pdf)] &#x2611; [2 | plane detection, aircraft 2d lidar]
* A Fast RANSAC–Based Registration Algorithm for Accurate Localization in Unknown Environments using LIDAR Measurements [[pdf](https://www.centropiaggio.unipi.it/sites/default/files/Localization-CASE07.pdf)] &#x2612;
* Hierarchical Plane Extraction (HPE): An Efficient Method For Extraction Of Planes From Large Pointcloud Datasets [[pdf](https://pdfs.semanticscholar.org/8217/61a207088e6015de845cc3f9e556e1c94be1.pdf)] &#x2612; [indoor setting]
* A Fast and Accurate Plane Detection Algorithm for Large Noisy Point Clouds Using Filtered Normals and Voxel Growing [[pdf](https://hal-mines-paristech.archives-ouvertes.fr/hal-01097361/document)] &#x2611; [2 | street scenes]
* SPLATNet: Sparse Lattice Networks for Point Cloud Processing CVPR 2018 [[pdf](https://arxiv.org/abs/1802.08275), [code](https://github.com/NVlabs/splatnet)] &#x2611; [1 | lattice spaces and scales convolution, 2D-3D (image-lidar) joint training, building tower vs building podium]
* PointContrast: Unsupervised Pre-training for 3D Point Cloud Understanding, 4D-VISION workshop at ECCV'2020 [[pdf](https://drive.google.com/file/d/1J1KqRQlvMeLThevw_2Erms5IiZWkEwde/view?usp=sharing), [workshop](https://sites.google.com/view/4dvision#h.u1ymvub25j59)] &#x2612;

## Object detection and Tracking
* Learning a Real-Time 3D Point Cloud Obstacle Discriminator via Bootstrapping [pdf](https://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.385.6290&rep=rep1&type=pdf)
* Terrain-Adaptive Obstacle Detection [[pdf](http://ais.informatik.uni-freiburg.de/publications/papers/suger16iros.pdf)]
* 3D Object Detection from Roadside Data Using Laser Scanners [[pdf](http://www-video.eecs.berkeley.edu/papers/JYT/spie-paper.pdf)]
* 3D Multiobject Tracking for Autonomous Driving : Masters thesis A S Abdul Rahman
* Motion-based Detection and Tracking in 3D LiDAR Scans [[pdf](http://ais.informatik.uni-freiburg.de/publications/papers/dewan16icra.pdf)]
* Lidar-histogram for fast road and obstacle detection [[pdf](http://www.chenliang.me/blog/wp-content/uploads/2017/07/lidarhistogram.pdf)] [[git](https://github.com/azurity/lidar-hist)] [-]
* End-to-end Learning of Multi-sensor 3D Tracking by Detection [pdf](https://arxiv.org/pdf/1806.11534.pdf) &#x2612; [tracking]
* Leveraging Heteroscedastic Aleatoric Uncertainties for Robust Real-Time LiDAR 3D Object Detection [[pdf](https://arxiv.org/abs/1809.05590), [video](https://www.youtube.com/watch?v=2DzH9COLpkU)]
* Deep tracking in the wild: End-to-end tracking using recurrent neural networks [[pdf](http://www.robots.ox.ac.uk/~mobile/Papers/2017_IJRR_Dequaire.pdf)]
* VoxelNet: End-to-End Learning for Point Cloud Based 3D Object Detection CVPR 2018 [[pdf](https://arxiv.org/abs/1711.06396), [code](https://github.com/tsinghua-rll/VoxelNet-tensorflow)]
* PIXOR: Real-time 3D Object Detection from Point Clouds CVPR 2018 [[pdf](https://arxiv.org/pdf/1902.06326.pdf)]
* Deep Multi-modal Object Detection and Semantic Segmentation for Autonomous Driving: Datasets, Methods, and Challenges [[pdf](https://arxiv.org/pdf/1902.07830.pdf)]
* Low resolution lidar-based multi-object tracking for driving applications [[pdf](https://upcommons.upc.edu/bitstream/handle/2117/113342/1924-Low-resolution-lidar-based-multi-object-tracking-for-driving-applications.pdf)]
* Patch Refinement -- Localized 3D Object Detection [[pdf](https://arxiv.org/abs/1910.04093)]
* PointPillars: Fast Encoders for Object Detection from Point Clouds CVPR 2019 [[pdf](http://openaccess.thecvf.com/content_CVPR_2019/papers/Lang_PointPillars_Fast_Encoders_for_Object_Detection_From_Point_Clouds_CVPR_2019_paper.pdf)]
* StarNet: Targeted Computation for Object Detection in Point Clouds NeurIPS 2019 ML4AD [[pdf](https://arxiv.org/abs/1908.11069)]
* PV-RCNN: Point-Voxel Feature Set Abstraction for 3D Object Detection CVPR 2020 [[pdf](http://openaccess.thecvf.com/content_CVPR_2020/papers/Shi_PV-RCNN_Point-Voxel_Feature_Set_Abstraction_for_3D_Object_Detection_CVPR_2020_paper.pdf)]
* LaserNet: An Efficient Probabilistic 3D Object Detector for Autonomous Driving CVPR 2019 [[pdf](http://openaccess.thecvf.com/content_CVPR_2019/papers/Meyer_LaserNet_An_Efficient_Probabilistic_3D_Object_Detector_for_Autonomous_Driving_CVPR_2019_paper.pdf)]
* Range Conditioned Dilated Convolutions for Scale Invariant 3D Object Detection 2020 [[pdf](https://arxiv.org/abs/2005.09927)]
* AFDet: Anchor Free One Stage 3D Object Detection [[pdf](https://arxiv.org/abs/2006.12671)]
* SA-SSD: Structure Aware Single-stage 3D Object Detection from Point Cloud (CVPR 2020) [[pdf](https://www4.comp.polyu.edu.hk/~cslzhang/paper/SA-SSD.pdf), [git](https://github.com/skyhehe123/SA-SSD)]
* Any Motion Detector: Learning Class-agnostic Scene Dynamics from a Sequence of LiDAR Point Clouds, ICRA 2020 [[pdf](https://arxiv.org/abs/2004.11647)]
* MVLidarNet: Real-Time Multi-Class Scene Understanding for Autonomous Driving Using Multiple Views [[link](https://www.youtube.com/watch?v=2ck5_sToayc), [video](https://www.youtube.com/watch?v=2ck5_sToayc)]
* Learning to Optimally Segment Point Clouds, ICRA 2020 [[pdf](https://arxiv.org/abs/1912.04976), [video](https://www.youtube.com/watch?v=wLxIAwIL870), [git](https://github.com/peiyunh/opcseg)]
* What You See is What You Get: Exploiting Visibility for 3D Object Detection [[pdf](https://arxiv.org/abs/1912.04986), [video](https://www.youtube.com/watch?v=497OF-otY2k), [project](https://www.cs.cmu.edu/~peiyunh/wysiwyg/index.html)]

## Classification/Supervised Learning
* PointNet: Deep Learning on Point Sets for 3D Classification and Segmentation [[link](http://stanford.edu/~rqi/pointnet/), [link2](http://stanford.edu/~rqi/pointnet2/)] &#x2611; [1 | segmentation, concat local and global features]
* SqueezeSeg: Convolutional Neural Nets with Recurrent CRF for Real-Time Road-Object Segmentation from 3D LiDAR Point Cloud [pdf](https://arxiv.org/pdf/1710.07368.pdf) &#x2612; [segment car, perdestrian and cyclist, preprocess of parking car]
* Improving LiDAR Point Cloud Classification using Intensities and Multiple Echoes [[pdf](https://hal.archives-ouvertes.fr/hal-01182604/document)] &#x2611; [1 | segmentation, not-drivable scenes]
```
-Parking lot, around a small water pond, and on an abandoned sport field. 
-The perceived scenes include trees, bushes, rocks, fences, and tall grass
```
* DepthCN: Vehicle Detection Using 3D-LIDAR and ConvNet [[pdf](http://home.isr.uc.pt/~cpremebida/files_cp/DepthCN_preprint.pdf)] &#x2611; [1 | ground removal, obstacles segmentation, 3D-2D projection]
* 3D Object Localisation with Convolutional Neural Networks [[Thesis](https://github.com/oscarmcnulty/gta-3d-dataset/blob/master/3D-object-localisation-with-cnns.pdf)] [-]
* SqueezeSegV2: Improved Model Structure and Unsupervised Domain Adaptation for Road-Object Segmentation from a LiDAR Point Cloud [[pdf](https://arxiv.org/pdf/1809.08495.pdf)] &#x2612; [segment car, perdestrian and cyclist, preprocess of parking car]
* PointSeg: Real-Time Semantic Segmentation Based on 3D LiDAR Point Cloud [[pdf](https://arxiv.org/pdf/1807.06288.pdf)] &#x2612; [segment car, perdestrian and cyclist, preprocess of parking car]
* Fast LIDAR-based Road Detection Using Fully Convolutional Neural Networks [[pdf](https://arxiv.org/abs/1703.03613)] &#x2611; [1 | top-view representation, FCN, urban roads]
* ChipNet: Real-Time LiDAR Processing for Drivable Region Segmentation on an FPGA [[pdf](https://arxiv.org/pdf/1808.03506.pdf)] &#x2611; [1 | spherical-view representation, convolution, simulated quantization, urban roads]


## Maps / Grids / HD Maps / Occupancy grids/ Prior Maps
* Hierarchies of Octrees for Efficient 3D Mapping [pdf](https://www.ais.uni-bonn.de/papers/IROS-2011_Wurm_Holz.pdf)
* Adaptive Resolution Grid Mapping using Nd-Tree [[ieee](https://ieeexplore.ieee.org/document/5980084)], [[pdf](https://www.researchgate.net/publication/224252536_Finding_the_adequate_resolution_for_grid_mapping_-_Cell_sizes_locally_adapting_on-the-fly), [video](https://www.youtube.com/watch?v=PYMlo8Wb6qE)]
* LIDAR-Data Accumulation Strategy To Generate High Definition Maps For Autonomous Vehicles [[link](https://ieeexplore.ieee.org/document/8170357/)]
* Long-term robot mapping in dynamic environments, Aisha Naima Walcott Thesis MIT 2011 [[link](https://dspace.mit.edu/handle/1721.1/66468)]
* Long-term 3D map maintenance in dynamic environments ICRA 2014 [[pdf](https://hal.archives-ouvertes.fr/hal-01143106/file/2014_Pomerleau_ICRA_Long-term.pdf), [video](https://www.youtube.com/watch?v=cMgLyLpnsoU)]
* Detection and Tracking of Moving Objects Using 2.5D Motion Grids ITSC 2015 [[pdf](http://a-asvadi.ir/wp-content/uploads/itsc15.pdf)]
* Autonomous Vehicle Navigation in Rural Environments without Detailed Prior Maps ICRA 2018 [[pdf](https://toyota.csail.mit.edu/sites/default/files/documents/papers/ICRA2018_AutonomousVehicleNavigationRuralEnvironment.pdf), [video](https://www.youtube.com/watch?v=v4qVNcGoMnI)]
* 3D Lidar-based Static and Moving Obstacle Detection in Driving Environments: an approach based on voxels and multi-region ground planes [[pdf](http://patternrecognition.cn/perception/negative2016a.pdf)]
* Spatio–Temporal Hilbert Maps for Continuous Occupancy Representation in Dynamic Environments [[pdf](https://papers.nips.cc/paper/6541-spatio-temporal-hilbert-maps-for-continuous-occupancy-representation-in-dynamic-environments.pdf)]
* Dynamic Occupancy Grid Prediction for Urban Autonomous Driving: A Deep Learning Approach with Fully Automatic Labeling [[pdf](https://arxiv.org/pdf/1705.08781.pdf)]
* Mobile Laser Scanned Point-Clouds for Road Object Detection and Extraction: A Review [[pdf](https://www.mdpi.com/2072-4292/10/10/1531)]
* Efficient Continuous-time SLAM for 3D Lidar-based Online Mapping [[pdf](https://www.ais.uni-bonn.de/papers/ICRA_2018_Droeschel.pdf)]
* DeLS-3D: Deep Localization and Segmentation with a 3D Semantic Map [[pdf](http://openaccess.thecvf.com/content_cvpr_2018/papers/Wang_DeLS-3D_Deep_Localization_CVPR_2018_paper.pdf)],[video](https://www.youtube.com/watch?v=M6lhkzKFEhA)]
* Recurrent-OctoMap: Learning State-based Map Refinement for Long-Term Semantic Mapping with 3D-Lidar Data [[pdf](https://arxiv.org/pdf/1807.00925.pdf)]
* HDNET: Exploiting HD Maps for 3D Object Detection [[pdf](http://proceedings.mlr.press/v87/yang18b/yang18b.pdf)]
* Mapping with Dynamic-Object Probabilities Calculated from Single 3D Range Scans ICRA 2018 [[pdf](http://ais.informatik.uni-freiburg.de/publications/papers/ruchti18icra.pdf)]

## End-To-End Learning
* Monocular Fisheye Camera Depth Estimation Using Semi-supervised Sparse Velodyne Data [[pdf](https://arxiv.org/pdf/1803.06192.pdf)]
* Fast and Furious: Real Time End-to-End 3D Detection, Tracking and Motion Forecasting with a Single Convolutional Net [[pdf](http://openaccess.thecvf.com/content_cvpr_2018/papers/Luo_Fast_and_Furious_CVPR_2018_paper.pdf)]

## Simulated pointclouds / Simulators 
* Virtual Generation of Lidar Data for Autonomous Vehicles Simulation of a lidar sensor inside a virtual world Bachelors Thesis 2017 [pdf](https://gupea.ub.gu.se/bitstream/2077/53342/1/gupea_2077_53342_1.pdf)
* A LiDAR Point Cloud Generator: from a Virtual World to Autonomous Driving ACM 2018 [[pdf](https://arxiv.org/abs/1804.00103)]
* Udacity based simulator [[link](http://wangyangevan.weebly.com/lidar-simulation.html), [git](https://github.com/EvanWY/USelfDrivingSimulator)]
* Tutorial on Gazebo to simulate raycasting from Velodyne lidar [[link](http://gazebosim.org/tutorials?tut=guided_i1)]
* Udacity Driving Dataset [[link](https://github.com/udacity/self-driving-car/tree/master/datasets)]
* Virtual KITTI [[link](http://www.europe.naverlabs.com/Research/Computer-Vision/Proxy-Virtual-Worlds)]
* SynthCity: A large-scale synthetic point cloud 2019 [[dataset](http://www.synthcity.xyz/), [pdf](https://arxiv.org/abs/1907.04758)]
* Precise Synthetic Image and LiDAR (PreSIL) Dataset for Autonomous Vehicle Perception [[link](https://uwaterloo.ca/waterloo-intelligent-systems-engineering-lab/projects/precise-synthetic-image-and-lidar-presil-dataset-autonomous)]
* Fast Synthetic LiDAR Rendering via Spherical UV Unwrapping of Equirectangular Z-Buffer Images 2020 [[pdf](https://arxiv.org/abs/2006.04345)]

## Lidar Datasets 
* nuScenes : public large-scale dataset for autonomous driving [[dataset](https://www.nuscenes.org/overview)]
    * nuScenes-lidarseg will be released in Q2 2020. [[link](https://www.nuscenes.org/lidarseg)]
* Ford Campus Vision and Lidar Data Set [[pdf](http://robots.engin.umich.edu/uploads/SoftwareData/Ford/ijrr2011.pdf), [dataset](http://robots.engin.umich.edu/SoftwareData/Ford)]
* Oxford RobotCar dataset [dataset](https://robotcar-dataset.robots.ox.ac.uk/) 1 Year, 1000km: The Oxford RobotCar Dataset [pdf](https://robotcar-dataset.robots.ox.ac.uk/images/robotcar_ijrr.pdf)
* LiDAR-Video Driving Dataset: Learning Driving Policies Effectively [[pdf](http://openaccess.thecvf.com/content_cvpr_2018/papers/Chen_LiDAR-Video_Driving_Dataset_CVPR_2018_paper.pdf)]
* KAIST Complex Urban Data Set Dataset [[dataset](http://irap.kaist.ac.kr/dataset/download_1.html)]
* Semantic 3D 2017 [dataset](http://www.semantic3d.net/) 
* Paris-Lille-3D: A Point Cloud Dataset for Urban Scene Segmentation and Classification [[pdf](http://openaccess.thecvf.com/content_cvpr_2018_workshops/papers/w40/Roynard_Paris-Lille-3D_A_Point_CVPR_2018_paper.pdf) [dataset](http://npm3d.fr/paris-lille-3d)]
* Semantic KITTI 2019 [[dataset](http://semantic-kitti.org/)]
* A*3D: An Autonomous Driving Dataset in Challeging Environments [[dataset](https://github.com/I2RDL2/ASTAR-3D)], [video](https://www.youtube.com/watch?v=QtK0VIywrmM&feature=youtu.be)]
* HD Map Dataset & Localization Dataset NAVER Labs : [[link](https://hdmap.naverlabs.com/dataset.html)]
* Argoverse by ARGO AI : Two public datasets supported by highly detailed maps to test, experiment, and teach self-driving vehicles how to understand the world around them. [[link](https://www.argoverse.org/)]
* Lyft dataset [[link](https://level5.lyft.com/dataset/)]
* SemanticPOSS: A Point Cloud Dataset with Large Quantity of Dynamic Instances [[link](http://www.poss.pku.edu.cn/semanticposs.html), [pdf](https://arxiv.org/abs/2002.09147)]
* A2D2 Audi dataset [[link](https://www.a2d2.audi/a2d2/en/dataset.html)]
* PandaSet : Public large-scale dataset for autonomous driving provided by Hesai & Scale. [[link](https://scale.com/open-datasets/pandaset)]
* Toronto-3D: A Large-scale Mobile LiDAR Dataset for Semantic Segmentation of Urban Roadways [[pdf](https://openaccess.thecvf.com/content_CVPRW_2020/papers/w11/Tan_Toronto-3D_A_Large-Scale_Mobile_LiDAR_Dataset_for_Semantic_Segmentation_of_CVPRW_2020_paper.pdf), [dataset](https://github.com/WeikaiTan/Toronto-3D)]

## Spatio-Temporal, Movement, Flow estimation in Pointclouds
* Rigid Scene Flow for 3D LiDAR Scans IROS 2016 [[pdf](https://europa2.informatik.uni-freiburg.de/files/dewan-16iros.pdf)]
* Deep Lidar CNN to Understand the Dynamics of Moving Vehicles [[pdf](http://www.iri.upc.edu/files/scidoc/2018-Deep-Lidar-CNN-to-Understand-the-Dynamics-of-Moving-Vehicles.pdf)]
* Learning motion field of LiDAR point cloud with convolutional networks [[link](https://www.sciencedirect.com/science/article/abs/pii/S016786551930176X)]
* Hallucinating Dense Optical Flow from Sparse Lidar for Autonomous Vehicles [[pdf](https://arxiv.org/pdf/1808.10542.pdf) [video](https://www.youtube.com/watch?v=94vQUwCZLxQ)]
* FlowNet3D: Learning Scene Flow in 3D Point Clouds CVPR 2019 [[pdf](https://zpascal.net/cvpr2019/Liu_FlowNet3D_Learning_Scene_Flow_in_3D_Point_Clouds_CVPR_2019_paper.pdf), [code](https://github.com/xingyul/flownet3d)]
* LiDAR-Flow: Dense Scene Flow Estimation from Sparse LiDAR and Stereo Images [[pdf](https://arxiv.org/abs/1910.14453v1)]
* 4D Spatio-Temporal ConvNets: Minkowski Convolutional Neural Networks CVPR 2019 [[pdf](https://zpascal.net/cvpr2019/Choy_4D_Spatio-Temporal_ConvNets_Minkowski_Convolutional_Neural_Networks_CVPR_2019_paper.pdf), [code](https://github.com/StanfordVL/MinkowskiEngine)]
* MeteorNet: Deep Learning on Dynamic 3D Point Cloud Sequences, ICCV 2019 [[pdf](http://openaccess.thecvf.com/content_ICCV_2019/papers/Liu_MeteorNet_Deep_Learning_on_Dynamic_3D_Point_Cloud_Sequences_ICCV_2019_paper.pdf)]
* DeepLiDARFlow: A Deep Learning Architecture For Scene Flow Estimation Using Monocular Camera and Sparse LiDAR 2020 [[pdf](https://arxiv.org/abs/2008.08136)]

## Advanced Topics/Other applications
**Tasks** : Upsampling, Domain adaptation Sim2Real, NAS, SSL, shape reconstruction, outlier extraction, Compression, Change detection, Domain Transfer
* Semantic Point Cloud Filtering, Masters thesis 2017 [link](https://ethz.ch/content/dam/ethz/special-interest/baug/igp/photogrammetry-remote-sensing-dam/documents/pdf/Student_Theses/MasterThesis_Stucker.pdf)
* PU-GAN: a Point Cloud Upsampling Adversarial Network ICCV 2019 [[pdf](https://arxiv.org/abs/1907.10844), [code](https://github.com/liruihui/PU-GAN)]
* Neural Architecture Search for Object Detection in Point Cloud [[blog](https://medium.com/seoul-robotics/neural-architecture-search-for-object-detection-in-point-cloud-f2d57a5953d5)], [[AutoDeepLabNAS paper](http://openaccess.thecvf.com/content_CVPR_2019/papers/Liu_Auto-DeepLab_Hierarchical_Neural_Architecture_Search_for_Semantic_Image_Segmentation_CVPR_2019_paper.pdf)]
* Weighted Point Cloud Augmentation for Neural Network Training Data Class-Imbalance [[pdf](https://arxiv.org/abs/1904.04094)]
* Quantifying Data Augmentation for LiDAR based 3D Object Detection [[pdf](https://arxiv.org/pdf/2004.01643v1.pdf)]
* Improving 3D Object Detection through Progressive Population Based Augmentation [[pdf(https://arxiv.org/abs/2004.00831)]
* 3D Object Detection From LiDAR Data Using Distance Dependent Feature Extraction VEHITS 2020 [[pdf](https://arxiv.org/abs/2003.00888)]
* Training a Fast Object Detector for LiDAR Range Images Using Labeled Data from Sensors with Higher Resolution ITSC 2019 [[pdf](https://arxiv.org/abs/1905.03066)]
* Performance of LiDAR object detection deep learning architectures based on artificially generated point cloud data from CARLA simulator 2019 [[pdf](https://ieeexplore.ieee.org/abstract/document/8864642/)]
* Efficient Learning on Point Clouds with Basis Point Sets ICCV 2019 [[pdf](https://openaccess.thecvf.com/content_ICCV_2019/papers/Prokudin_Efficient_Learning_on_Point_Clouds_With_Basis_Point_Sets_ICCV_2019_paper.pdf)]
* Mastering Data Complexity for Autonomous Driving with Adaptive Point Clouds for Urban Environments 2017 [[pdf](https://www.researchgate.net/publication/318093493_Mastering_Data_Complexity_for_Autonomous_Driving_with_Adaptive_Point_Clouds_for_Urban_Environments)]
* Visually aided changes detection in 3D lidar based reconstruction 2015 [[Thesis](https://www.politesi.polimi.it/bitstream/10589/112343/3/tesi-Postica.pdf)]
* Fast Polar Attentive 3D Object Detection on LiDAR Point Clouds ML4AD 2021 [pdf](https://ml4ad.github.io/files/papers2021/Fast%20Polar%20Attentive%203D%20Object%20Detection%20on%20LiDAR%20Point%20Clouds.pdf)

## Implicit representations
* Neural Implicit Embedding for Point Cloud Analysis CVPR 2020 [[pdf](https://openaccess.thecvf.com/content_CVPR_2020/papers/Fujiwara_Neural_Implicit_Embedding_for_Point_Cloud_Analysis_CVPR_2020_paper.pdf)]
* DeepSDF: Learning Continuous Signed Distance Functions for Shape Representation [[pdf](https://arxiv.org/abs/1901.05103)]

## Domain adaptation and domain transer
* Complete & Label: A Domain Adaptation Approach to Semantic Segmentation of LiDAR Point Clouds 2020 [[pdf](https://arxiv.org/abs/2007.08488)]
* PointDAN: A Multi-Scale 3D Domain Adaption Network for Point Cloud Representation [[pdf](https://papers.nips.cc/paper/8940-pointdan-a-multi-scale-3d-domain-adaption-network-for-point-cloud-representation.pdf)]
* Domain Transfer for Semantic Segmentation of LiDAR Data using Deep Neural Networks IROS 2020 [[pdf](http://ras.papercept.net/images/temp/IROS/files/0060.pdf), [video](https://www.youtube.com/watch?v=EkCO36zX6OI)]
* Domain Adaptation for Vehicle Detection from Bird's Eye View LiDAR Point Cloud Data ICCVW 2019 [pdf](http://openaccess.thecvf.com/content_ICCVW_2019/papers/TASK-CV/Saleh_Domain_Adaptation_for_Vehicle_Detection_from_Birds_Eye_View_LiDAR_ICCVW_2019_paper.pdf)

## Self-supervised learning
* Self-Supervised Deep Learning on Point Clouds by Reconstructing Space NeurIPS 2019 [[pdf](https://arxiv.org/abs/1901.08396)]
* SegContrast: 3D Point Cloud Feature Representation Learning RAL-ICRA'22 [video](https://www.youtube.com/watch?v=kotRb_ySnIw), [pdf](http://www.ipb.uni-bonn.de/pdfs/nunes2022ral-icra.pdf)
* Self-supervised Point Cloud Prediction Using 3D Spatio-temporal CNNs CORL 2021 [pdf](https://www.ipb.uni-bonn.de/wp-content/papercite-data/pdf/mersch2021corl.pdf) 


## Graphs and Pointclouds
* Detection of closed sharp edges in point clouds using normal estimation and graph theory CAD 2007 [[link](https://www.sciencedirect.com/science/article/abs/pii/S0010448506002260)]
* Dynamic Edge-Conditioned Filters in Convolutional Neural Networks on Graphs CVPR 2017 [[pdf](https://openaccess.thecvf.com/content_cvpr_2017/papers/Simonovsky_Dynamic_Edge-Conditioned_Filters_CVPR_2017_paper.pdf), [vide](https://www.youtube.com/watch?v=THOoeNMwUIk)]
* Large-scale Point Cloud Semantic Segmentation with Superpoint Graphs CVPR2018 [[pdf](http://openaccess.thecvf.com/content_cvpr_2018/papers/Landrieu_Large-Scale_Point_Cloud_CVPR_2018_paper.pdf)]
* ConvPoint: continuous convolutions for cloud processing Eurographics 3DOR, 2019 [[pdf](https://arxiv.org/abs/1904.02375), [code](https://github.com/aboulch/ConvPoint)]
* Point Cloud Oversegmentation with Graph-Structured Deep Metric Learning [[CVPR Workshop 2019](https://scene-understanding.com/papers/point_cloud_oversegmentation__CVPR_workshop_-1.pdf)], [video](https://www.youtube.com/watch?v=bKxU03tjLJ4&feature=youtu.be)
* Dynamic Graph CNN for Learning on Point Clouds [[pdf](https://arxiv.org/abs/1801.07829), [project](https://liuziwei7.github.io/projects/DGCNN)] TOG 2019

## Large-scale pointcloud Algorithms (vs scan based)
* Deep Parametric Continuous Convolutional Neural Networks CVPR 2018 [[pdf](http://openaccess.thecvf.com/content_cvpr_2018/papers_backup/Wang_Deep_Parametric_Continuous_CVPR_2018_paper.pdf)]
* PointNet++: Deep Hierarchical Feature Learning on Point Sets in a Metric Space NeurIPS 2017 [[pdf](https://papers.nips.cc/paper/7095-pointnet-deep-hierarchical-feature-learning-on-point-sets-in-a-metric-space.pdf), [code](https://github.com/charlesq34/pointnet2)], [semantic seg code](https://github.com/mathieuorhan/pointnet2_semantic)
* Classification of Point Cloud for Road Scene Understanding with Multiscale Voxel Deep Network [Slides](https://project.inria.fr/ppniv18/files/2018/10/presentation.pdf)
* Semantic Segmentation of 3D point Clouds Loic Landireu [[Slides](http://bezout.univ-paris-est.fr/wp-content/uploads/2019/04/Landrieu_GT_appr_opt.pdf)]
* KPConv: Flexible and Deformable Convolution for Point Clouds [[pdf](https://arxiv.org/abs/1904.08889), [git](https://github.com/HuguesTHOMAS/KPConv)]
* RandLA-Net: Efficient Semantic Segmentation of Large-Scale Point Clouds [[pdf](https://openaccess.thecvf.com/content_CVPR_2020/html/Hu_RandLA-Net_Efficient_Semantic_Segmentation_of_Large-Scale_Point_Clouds_CVPR_2020_paper.html), [git](https://github.com/QingyongHu/RandLA-Net)]
* Cylinder3D: An Effective 3D Framework for Driving-scene LiDAR Semantic Segmentation CVPR 2021 [pdf](https://arxiv.org/abs/2008.01550)

## 4D Panoptic LiDAR Segmentation
* Panoptic nuScenes: A Large-Scale Benchmark for LiDAR Panoptic Segmentation and Tracking 2021 [video](https://www.youtube.com/watch?v=CG5dQbISK1g), [pdf](https://arxiv.org/abs/2109.03805), nuscenes [benchmark](https://www.nuscenes.org/panoptic?externalData=all&mapData=all&modalities=Any)
* 4D Panoptic LiDAR Segmentation CVPR 2021 [pdf](https://openaccess.thecvf.com/content/CVPR2021/papers/Aygun_4D_Panoptic_LiDAR_Segmentation_CVPR_2021_paper.pdf), [project](https://mehmetaygun.github.io/4DPLS.html)
* Contrastive Instance Association for 4D Panoptic Segmentation using Sequences of 3D LiDAR Scans 2022 RAL [pdf](https://www.ipb.uni-bonn.de/wp-content/papercite-data/pdf/marcuzzi2022ral.pdf), [video](https://www.youtube.com/watch?v=XXwiadwjLp4)

## Embedded/Resource constrained pointcloud processing
* Sparse PointPillars: Maintaining and Exploiting Input Sparsity to Improve Runtime on Embedded Systems [pdf](https://vedder.io/publications/sparse_point_pillars_iros_2022.pdf), [video](https://www.youtube.com/watch?v=zuLboHg3GLA)
* IBB-Net: Fast Iterative Bounding Box Regression for Detection on Point Clouds, Brendan Miller, 2020 CMU [masters thesis](https://www.ri.cmu.edu/wp-content/uploads/2020/06/MSR_Thesis.pdf)
* Fast 3-D Urban Object Detection on Streaming Point Clouds [[pdf](https://projet.liris.cnrs.fr/imagine/pub/proceedings/ECCV-2014/workshops/w15/Paper%202.pdf)]
* StrObe: Streaming Object Detection from LiDAR Packets [pdf](https://arxiv.org/abs/2011.06425), [video](https://www.youtube.com/watch?v=18uY9P6Y9Ys)
* PolarStream: Streaming Lidar Object Detection and Segmentation with Polar Pillars NeurIPS 2021 [pdf](https://arxiv.org/abs/2106.07545), [video](https://youtu.be/wGgO8SKwixo?t=1199), [code](https://github.com/motional/polarstream)
* RAD: Realtime and Accurate 3D Object Detection on Embedded Systems CVPRW 2021 [pdf](https://openaccess.thecvf.com/content/CVPR2021W/WAD/papers/Aghdam_RAD_Realtime_and_Accurate_3D_Object_Detection_on_Embedded_Systems_CVPRW_2021_paper.pdf)
* BEVDetNet: Bird’s Eye View LiDAR Point Cloud based Real-time 3D Object Detection for Autonomous Driving ITSC 2021 [pdf](https://arxiv.org/abs/2104.10780)
* Streaming Object Detection for 3-D Point Clouds 2020 [pdf](https://arxiv.org/abs/2005.01864)
 
## Tools/SW/Packages
* Python bindings for Point Cloud Library [[git](https://github.com/strawlab/python-pcl)] 
* Open3D [[link](http://www.open3d.org/)]
* pyntcloud [[link](https://github.com/daavoo/pyntcloud)]
* PyVista [[link](https://github.com/pyvista/pyvista)]
* torch-points3d : Pytorch framework for doing deep learning on point clouds  [[link](https://torch-points3d.readthedocs.io/en/latest/)]
* Geometric Deep Learning Extension Library for [PyTorch [link](https://pytorch-geometric.readthedocs.io/en/latest/)]
* kaolin : A PyTorch Library for Accelerating 3D Deep Learning Research [[link](https://github.com/NVIDIAGameWorks/kaolin/)]
* PyTorch3D : FAIR's library of reusable components for deep learning with 3D data [[link](https://pytorch3d.org/)]
* PCDet Toolbox in PyTorch for 3D Object Detection from Point Cloud [[link](https://github.com/sshaoshuai/PCDet)]
* pointcloudset: Efficient analysis of large datasets of point clouds recorded over time [[link](https://github.com/virtual-vehicle/pointcloudset)]
