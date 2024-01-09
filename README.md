# Intro to Artsy Coding
- This is a collection of exercises I found useful while learning coding for "visually artsy" purposes
- In graphics-related work there is always a higher-level and lower-level than you are comfortable with
  - The very highest level is specialized software like Blender, Houdini, Unity's VFX graph, etc.
  - The very low level is a layer above hardware, with Vulcan, DirectX, Metal, and emerging ones like WebGPU

- While it's cool to be a wizard at either extreme, I feel like it's useful for beginners to get comfortable with the middle-ground first
  - Ultimately, tools at any level are just *tools*, they are in the way between *you* and *the thing you want to make*
  - I want this set of exercises to cover a lot of areas while not over-shadowing the actual thing you want to make
  > This is mainly why the following exercises are made in Unity. I do not like their company's recent behavior, but you choose tools based on what you want to accomplish (plus I get it for free so ¯\\_(ツ)_/¯)
  > 
  > If you are more inclined for higher-level and more pipelined work, Unreal provides a lot of tooling for shaders and working with assets in general. However tweaking their render pipeline at the base level (i.e. adding more render textures and defining render passes) is pretty unintuitive.

- Ideally, you would be able to know what to search for (and maybe also where) when you want to make something visually artsy
  - There are way better tutorials for each specific part of the high-to-low-level spectrum
  - There are also great resources for theory without necessarily the implementation

- Ultimately, the set of exercises are chosen from my own path and by no means cover any professional field. I do this as hobby not my job :)

## Prerequisites
- Please install Unity Editor LTS 2022.3.16f1

## Format
- Unit folders are numbered in order, they are summarized below
- Each unit folder contains at least one Unity project that will be **capitalized**
- All other files are supplements that you can take a look at, for example README's

## Maths
- You *will* need [Desmos](https://www.desmos.com/calculator) at some point of you life
  - Familiarize yourself with all exponential, trig, "number theory" functions like `floor` and `ceil`, and statistic distributions
- Coordinates and vectors
  - Barycentric coordinates
  - Time (not actual time, just the `t` variable in curves)
  - Spaces and transforming between them
    - Handedness and conventions
- Noise
  - Perlin noise
- Color space
  - Implementing HSV
  - Implementing OKLab

## Fragment Shaders
- Fragment shaders
- Maths in HLSL
- Texture sampling: texels, edge behavior, interpolation methods
- Cursed flat shader: calculus in shader programming and when they can be useful
- Compute shader noise
  - Challenge: 3D noise

## Manipulating Shapes
- From grid to UV sphere
- The Hand: animating a procedural mesh
- Basics of vertex data
- Vertex shaders
- Touching grass: GPU instancing
  - Challenge: adding wind

## Not-Necessarily-Post Processing
- Budget water: rendering order and sampling from prior renders
- Stencil shader

## Rendering Pipelines
- Stages of URP
- Writing an SRP feature

## VFX Graph Intro
> ??? I don't actually know VFX lol

## Reading and Replication
- Getting a hang of repliating papers
