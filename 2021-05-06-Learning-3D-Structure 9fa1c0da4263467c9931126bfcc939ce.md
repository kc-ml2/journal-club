# 2021-05-06-Learning-3D-Structure

## Introduction

<backgrounds>

- 3D data is interesting topics in Machine Learning
    - There are diverse research fields in 3D ML
- Unlike Image, 3D data has various representations.
    - There are diverse NN for 3D data

        ![2021-05-06-Learning-3D-Structure%209fa1c0da4263467c9931126bfcc939ce/Untitled.png](2021-05-06-Learning-3D-Structure%209fa1c0da4263467c9931126bfcc939ce/Untitled.png)

        - Voxels
            - Using Octree : O-CNN
            - Using Sparse Window for only tracking surface : Sparse-ConvNet
        - Mesh
            - Using relationship between two adjacent region + pooling : MeshCNN
            - Using  adjacent mesh + geometric length : DualConvMeshNet
        - Point
            - PointNet + PointNet++

<How gets 3D-data>

- LiDAR : Point Cloud
- CAD model : Primitives + Mesh(Rendered)
    - Primitive examples

    ![2021-05-06-Learning-3D-Structure%209fa1c0da4263467c9931126bfcc939ce/Untitled%201.png](2021-05-06-Learning-3D-Structure%209fa1c0da4263467c9931126bfcc939ce/Untitled%201.png)

- Multi-View Camera, etc.

→ Point Cloud and Mesh

<Given 3D Datasets>

- ShapeNet
    - [https://shapenet.org/](https://shapenet.org/)
    - 51k models, 55 categories

        → CAD models

        ![2021-05-06-Learning-3D-Structure%209fa1c0da4263467c9931126bfcc939ce/Untitled%202.png](2021-05-06-Learning-3D-Structure%209fa1c0da4263467c9931126bfcc939ce/Untitled%202.png)

        ![2021-05-06-Learning-3D-Structure%209fa1c0da4263467c9931126bfcc939ce/Untitled%203.png](2021-05-06-Learning-3D-Structure%209fa1c0da4263467c9931126bfcc939ce/Untitled%203.png)

- ShapeNet classification
    - Get input 3D model and predict the true label
- ShapeNet segmentation
    - Get input 3D model and segment its parts

        ![2021-05-06-Learning-3D-Structure%209fa1c0da4263467c9931126bfcc939ce/Untitled%204.png](2021-05-06-Learning-3D-Structure%209fa1c0da4263467c9931126bfcc939ce/Untitled%204.png)

→ ModelNet40 : [https://paperswithcode.com/sota/3d-point-cloud-classification-on-modelnet40](https://paperswithcode.com/sota/3d-point-cloud-classification-on-modelnet40)

## PointNet & PointNet++

PointNet++(2017) : [https://arxiv.org/abs/1706.02413](https://arxiv.org/abs/1706.02413)

PointNet(2016) : [https://arxiv.org/abs/1612.00593](https://arxiv.org/abs/1612.00593)

<PointNet>

- Learning Point Cloud input
    - do classification and segmentation

        ![2021-05-06-Learning-3D-Structure%209fa1c0da4263467c9931126bfcc939ce/Untitled%205.png](2021-05-06-Learning-3D-Structure%209fa1c0da4263467c9931126bfcc939ce/Untitled%205.png)

        ![2021-05-06-Learning-3D-Structure%209fa1c0da4263467c9931126bfcc939ce/Untitled%206.png](2021-05-06-Learning-3D-Structure%209fa1c0da4263467c9931126bfcc939ce/Untitled%206.png)

<PointNet++>

- Using Hierarchy to better represenetation

    ![2021-05-06-Learning-3D-Structure%209fa1c0da4263467c9931126bfcc939ce/Untitled%207.png](2021-05-06-Learning-3D-Structure%209fa1c0da4263467c9931126bfcc939ce/Untitled%207.png)

<A Point Set Generation Network for 3D object reconstruction from a Single Image>

- link: [https://arxiv.org/abs/1612.00603](https://arxiv.org/abs/1612.00603)

# StructureNet Vs. GRASS

→ Both use Hierarchy of the structures to learn the feature

→ GRASS uses binary, but StructureNet uses n-ary graph

## StructureNet

StructureNet (2019) : [https://arxiv.org/abs/1908.00575](https://arxiv.org/abs/1908.00575)

PartNet(2018) : [https://arxiv.org/abs/1812.02713](https://arxiv.org/abs/1812.02713) 

- PartNet is dataset + little test
- Used in StructureNet for performance test

StructEdit(2019) : [https://arxiv.org/abs/1911.11098](https://arxiv.org/abs/1911.11098)

## GRASS

GRASS(2017) : [https://arxiv.org/abs/1705.02090](https://arxiv.org/abs/1705.02090)