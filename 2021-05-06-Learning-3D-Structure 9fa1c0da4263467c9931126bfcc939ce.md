# 2021-05-06-Learning-3D-Structure

## Introduction

<backgrounds>

- 3D data is interesting topics in Machine Learning
    - There are diverse research fields in 3D ML
- Unlike Image, 3D data has various representations.
    - There are diverse NN for 3D data

        
        ![Untitled](https://user-images.githubusercontent.com/65122489/116973546-adefb700-acf7-11eb-8bb4-ac56c04f2bd3.png)

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

    ![Untitled 1](https://user-images.githubusercontent.com/65122489/116973492-9dd7d780-acf7-11eb-801b-68321f8b00bb.png)

- Multi-View Camera, etc.

→ Point Cloud and Mesh

<Given 3D Datasets>

- ShapeNet
    - [https://shapenet.org/](https://shapenet.org/)
    - 51k models, 55 categories

        → CAD models

        ![Untitled 2](https://user-images.githubusercontent.com/65122489/116973496-9fa19b00-acf7-11eb-9929-ef70c6bf82f7.png)
        ![Untitled 3](https://user-images.githubusercontent.com/65122489/116973505-a203f500-acf7-11eb-8989-85b1865e6f35.png)

- ShapeNet classification
    - Get input 3D model and predict the true label
- ShapeNet segmentation
    - Get input 3D model and segment its parts

        ![Untitled 4](https://user-images.githubusercontent.com/65122489/116973508-a29c8b80-acf7-11eb-8294-f051dcc71fae.png)

→ ModelNet40 : [https://paperswithcode.com/sota/3d-point-cloud-classification-on-modelnet40](https://paperswithcode.com/sota/3d-point-cloud-classification-on-modelnet40)

## PointNet & PointNet++

PointNet++(2017) : [https://arxiv.org/abs/1706.02413](https://arxiv.org/abs/1706.02413)

PointNet(2016) : [https://arxiv.org/abs/1612.00593](https://arxiv.org/abs/1612.00593)

<PointNet>

- Learning Point Cloud input
    - do classification and segmentation

        
        ![Untitled 5](https://user-images.githubusercontent.com/65122489/116973518-a6301280-acf7-11eb-90c2-3da6cf329383.png)
        ![Untitled 6](https://user-images.githubusercontent.com/65122489/116973523-a7f9d600-acf7-11eb-9e0e-736a324e62c0.png)

<PointNet++>

- Using Hierarchy to better represenetation

    ![Untitled 7](https://user-images.githubusercontent.com/65122489/116973530-a9c39980-acf7-11eb-8ee2-b46578282889.png)

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
