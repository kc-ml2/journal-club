# 2021-05-06-Learning-3D-Structure

## Introduction

<backgrounds>

- 3D data is interesting topics in Machine Learning
    - There are diverse research fields in 3D ML
- Unlike Image, 3D data has various representations.
    - There are diverse NN for 3D data

        ![Untitled 1](https://user-images.githubusercontent.com/65122489/116973492-9dd7d780-acf7-11eb-801b-68321f8b00bb.png)


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

    ![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/3333d189-6044-47bf-b30e-3b1cfe5f84fe/Untitled.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/3333d189-6044-47bf-b30e-3b1cfe5f84fe/Untitled.png)

- Multi-View Camera, etc.

→ Point Cloud and Mesh

<Given 3D Datasets>

- ShapeNet
    - [https://shapenet.org/](https://shapenet.org/)
    - 51k models, 55 categories

        → CAD models

        ![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/798fb5fe-87cd-4f0a-955c-8e4930329042/Untitled.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/798fb5fe-87cd-4f0a-955c-8e4930329042/Untitled.png)
        ![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/8f30febc-f8d7-4b10-a5c6-97c9a6d64e47/Untitled.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/8f30febc-f8d7-4b10-a5c6-97c9a6d64e47/Untitled.png) 

- ShapeNet classification
    - Get input 3D model and predict the true label
- ShapeNet segmentation
    - Get input 3D model and segment its parts

        ![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/1f827424-519d-485f-aafd-2b9445d80c34/Untitled.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/1f827424-519d-485f-aafd-2b9445d80c34/Untitled.png)

→ ModelNet40 : [https://paperswithcode.com/sota/3d-point-cloud-classification-on-modelnet40](https://paperswithcode.com/sota/3d-point-cloud-classification-on-modelnet40)

## PointNet & PointNet++

PointNet++(2017) : [https://arxiv.org/abs/1706.02413](https://arxiv.org/abs/1706.02413)

PointNet(2016) : [https://arxiv.org/abs/1612.00593](https://arxiv.org/abs/1612.00593)

<PointNet>

- Learning Point Cloud input
    - do classification and segmentation

        ![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/a8696cd6-c735-429a-b867-4db759a0abc8/Untitled.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/a8696cd6-c735-429a-b867-4db759a0abc8/Untitled.png)
        ![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/d1b423cf-1d30-48ca-9afa-8755ce9982be/Untitled.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/d1b423cf-1d30-48ca-9afa-8755ce9982be/Untitled.png)

<PointNet++>

- Using Hierarchy to better represenetation

    ![https://s3-us-west-2.amazonaws.com/secure.notion-static.com/5f623b0e-fe97-4bcd-8dfd-4e535d72e114/Untitled.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/5f623b0e-fe97-4bcd-8dfd-4e535d72e114/Untitled.png)

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
