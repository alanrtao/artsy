# Intro to Artsy Coding
## What's Artsy Coding?
- This is a collection of exercises I found useful while learning coding for artistic (visual) purposes
- I will call the topic "artsy coding" to distance from several other terms
  - *Procedural art / Procedurally generated art* has several associations I don't like
  - *Technical art* is an umbrella term in game development that is not fully addressed by this set
  - *Graphics programming* are more low-level (close to hardware / data flow) than most of the exercises
  - I am not going to even attempt to call this "artistic" as I am just a hobbyist
- The main goal is to get you familiar with some jargon people use when making their computers show fancy pictures, as well as getting a *feel* of the maths
  - When doing shader programming and other non-physically-based effects, it is crucial to be able to imagine different functions and pick the right ones
- The set of exercises are chosen from my own experience, and I write them as straightforward as possible because there can be a *lot* of wasted steps when learning to art
 
## Numbers
- You *will* need [Desmos](https://www.desmos.com/calculator) at some point of you life
  - Familiarize yourself with all exponential, trig, "number theory" functions like `floor` and `ceil`, and statistic distributions
- Coordinates and vectors
  - Barycentric coordinates
  - Time (not actual time, just the `t` variable in curves)
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
- The Hand
- Basics of vertex data
- Vertex shaders
- Touching grass: GPU instancing

## Not-Necessarily-Post Processing
- Budget water: rendering order and sampling from prior renders
- Stencil shader
