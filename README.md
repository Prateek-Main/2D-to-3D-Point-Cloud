# Project Title: Converting 2D Images to 3D Point Cloud using MiDaS Model

## Description:
This project aims to convert 2D images into 3D point clouds using the MiDaS (Mixed Data Supervision) model, leveraging the Open3D library for visualization. The process involves utilizing the depth estimation capabilities of the MiDaS model to infer depth information from 2D images, which is then transformed into a 3D point cloud representation.

## Key Components:
- **MiDaS Model**: Implemented using PyTorch, the MiDaS model is utilized for depth estimation from 2D images. The model, available in various sizes, allows for flexible trade-offs between accuracy and speed.
- **Open3D Library**: Open3D is employed for visualizing the generated 3D point clouds and manipulating point cloud data. It provides tools for efficient point cloud processing and visualization.
- **Depth Estimation**: The MiDaS model infers depth maps from input images, providing depth information for each pixel. These depth maps are then used to construct the 3D point clouds.
- **Point Cloud Generation**: The depth maps are converted into 3D point clouds by associating each pixel's depth value with its corresponding spatial coordinates in 3D space. This process involves camera calibration parameters and geometric transformations.
- **Visualization**: Two types of visualizations are provided: a colored point cloud representing the 3D structure of the scene and a heatmap representation depicting the depth distribution within the scene.

## Implementation:
The project utilizes Python programming language and relevant libraries including PyTorch for the MiDaS model, Open3D for point cloud processing, and NumPy for array manipulations. The implementation involves loading the input image, processing it through the MiDaS model to obtain depth maps, and then converting these depth maps into 3D point clouds. Finally, the generated point clouds are visualized using Open3D.

## Output Presentation:
The project output consists of:
1. **Depth Image Heatmap**: A visualization of the depth map obtained from the input image, providing a grayscale representation of depth values.
   <img width="546" alt="Screenshot 2024-05-12 at 10 00 52 PM" src="https://github.com/Prateek-Main/2D-to-3D-Point-Cloud/assets/114331206/5e45dfd5-88a4-445d-a186-defc58b47036">
2. **Colored Point Cloud Video**: A dynamic visualization of the 3D point cloud, with each point colored based on its depth value, offering a comprehensive view of the scene's spatial structure.
   ![Colored Point Cloud Video]()
3. **Heatmap Point Cloud Video**: A dynamic representation of the 3D point cloud with heatmap coloring, visually conveying the depth distribution within the scene.
   ![Heatmap Point Cloud Video]()

## Conclusion:
By leveraging deep learning-based depth estimation and 3D point cloud generation techniques, this project offers a novel approach to convert 2D images into rich 3D representations, enabling applications in various domains including computer vision, robotics, and augmented reality.
