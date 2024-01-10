# Intro to Artsy Coding
- This is a collection of exercises I found useful while learning coding for "visually artsy" purposes
  - I'm just a hobbyist so this does *not* cover any professional field like tech art / graphics programming. Please talk to a professional instead!

- In graphics-related work there is always a higher-level and lower-level than you are comfortable with
  - The very highest level is specialized software like Blender, Houdini, Unity's VFX graph, etc.
  - The very low level is a layer above hardware, with Vulcan, DirectX, Metal, and emerging one

If you are more inclined for higher-level and more pipelined work, Unreal provides a lot of tooling for shaders and working with assets in general. However tweaking their render pipeline at the base level (i.e. adding more render textures and defining render passes) is pretty unintuitive.

Godot is cool and pretty customizable but their language is dynamically typed and sample code could be confusing.s like WebGPU

- While it's cool to be a wizard at either extreme, I feel like it's useful for beginners to get comfortable with the middle-ground first
  - Ultimately, tools at any level are just *tools*, they are in the way between *you* and *the thing you want to make*
  - I want this set of exercises to cover a lot of areas while not over-shadowing the actual thing you want to make
  > This is mainly why the following exercises are made in Unity.
  > 
  > Unreal provides a lot of tooling for higher-level work, but tweaking their render pipeline at the base level (i.e. adding more render textures and defining render passes) is pretty unintuitive.
  > 
  > Godot is cool and pretty customizable but their language is dynamically typed and sample code could be confusing.

- A lot of stuff you do in graphics is combining other people's ideas and then implementing them, so I will structure this set of exercises as closely to that process as possible instead of handholding every single step

- Have fun! :)

## Prerequisites
- Please install Unity Editor LTS 2022.3.16f1
- Basic terminology in Unity
  - A **scene** is a collection of objects a viewer is exposed to at a time
    - Scenes are always 3D in Unity, Unity 2D is still in 3D, just ignoring on dimension
  - A **game object** is an object placed in the scene
    - It doesn't necessarily need to have any visible form, but it does have a *transform* describing its position, orientation, and size
    - Game objects have **components** attached to them, which *do not* have a separate transform (this aspect is different from UE's components)
    - A game object can be attached to one other game object, called its **parent**, one parent can have multiple **children**
      - Unlike components, child game objects can have a *relative* transform based on it's parent
  - A **prefab** is a game object saved in the project without being attached to any scene
    - They can be spawned into any scene
  - A **scriptable object** is pure data living in the project itself without being attached to any scene
    - Game objects can refer to scriptable objects, and scriptable objects can access game objects if they're coded to do so

## Format
- Unit folders are numbered in order below, they are summarized in this README and elaborated in each repsective folder
  - Each unit folder contains at least one Unity project that will be capitalized
  - All other supplementary files are lower case

## Math
- Functions
  - The "feel" and "cost" of functions
  - Time and "time"
- Coordinates and vectors
  - Spaces and transforming between them
  - Non-rectangular coordinates (namely barycentric)
- Noise
  - Perlin noise
  - Worley noise
- Color space
  - Implementing HSV
  - Implementing OKLab

## Fragment Shaders

> I am placing this section before the next as it transitions well from the previous section, but technically speaking fragment shaders come *after* vertex shaders which is in the next section.

- Fragment shaders and HLSL
- Texture sampling: texels, edge behavior, interpolation methods
- (Differential) calculus in shaders
- Compute shaders
  - Blur and other kernels
  - Revisiting noise

## Shapes and Models
- From grid to UV sphere
- The Hand: animating a procedural mesh
- Vertex Data
- Vertex shaders
- Touching grass: GPU instancing
  - Challenge: adding wind

## Unity Shader Graph
- Comparing it to HLSL
- Using HLSL within Shader Graph

## Not-Necessarily-Post Processing
- Budget water
- Stencil shader

## Rendering Pipelines
- Stages of URP
- Writing an SRP feature

## VFX Graph Intro
> ??? I don't actually know VFX lol

## Reading and Replication
- Getting a hang of repliating papers
