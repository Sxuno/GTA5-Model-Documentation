# GTA5-Model-Documentation

# Basics

## Programs

GTA 5

[OpenV](https://openiv.com/)

[CodeWalker](https://github.com/dexyfex/CodeWalker/)

[Archive Fix](https://gtaforums.com/topic/871168-affix-fix-your-rpf-archives-and-work-without-openiv/)

Autodesk 3ds Max

*Addonscript*
   
[GIMS Evo](https://de.gta5-mods.com/tools/gims-evo-with-gta-v-support/)

[Blender](https://www.blender.org/)

*Pythonscript*

[Openformat-to-obj](https://github.com/hedgehog90/openformat-to-obj/)

[Krita](https://krita.org/en/)

[Awesomebump](https://github.com/kmkolasinski/AwesomeBump/)

# Data file types

**Rpf**

> Archivefile, wich can contains different datafiles. Existing RPF can be deactivated throu content.xml in an dlc.

**Ytype**

Asset definition file

Definition file with xml case sensitive syntax which providing additional data for the system like draw boundings, physics directorie and more.

*Assettypes*
>
>  Drawable
>
>      Defintion of an object base on a ydr model.
>
>   Milo
>
>      Definition of zones and models to load. It uses Entity definition to build an array which is be used to set items to zones.
>
>   Entity
>
>      Definition of objects which are used in Milo.

**Ydr**

   Model file

**Ybn**

   Static collision file is an additional model to an existing one. It contains mostly simple box collisions which matches the geometry of its parent model.

**Ytd**

   Texturedictionary file

**Ymap**

   Map position definition file

**Xml**

   System definition file contains data in xml which are directly handled by the system. These files are case sensetive in its structure.

# Model

## Basics

   Normal direction

   Vertexcount

   Material

   Meshmodifier

## Create

## Export

# Collision

## Collision types

### Embeded Collision

> On map load it will be loaded last, blocks flags only. Maximum allowed vertecies +32k.

### Static Collision

> On map loading it will be loaded first, blocks rain and snow automaticly.

## Collision Flaggs

Flags 1                    | Flags 2 
------------               | -------------
Defines group of collision | Defines group of collision to interact with
Animal                     | Animal
Animal Ragdoll             | Animal Ragdoll
Explosion                  | Exlosion
Foliage                    | Foiage
Forklift forks             | Forklift forks
Glass                      | Glass
Map animal                 | Map animal
Map cover                  | Map cover
Map deep surface           | Map deep surface
Map dynamic                | Map dynamic
Map river                  | Map river
Map stairs                 | Map stairs
Map vehicle                | Map vehicle
Map weapon                 | Map weapon
Object                     | Object
Object env cloth           | Object env cloth
Ped                        | Ped
Pickup                     | Pickup
Plant                      | Plant
Projectile                 | Projectile
Ragdoll                    | Ragdoll
Smoke                      | Smoke
Test ai                    | Test ai
Test camera                | Test camera
Test script                | Test script
Test vehicle wheel         | Test vehicle wheel
Test weapon                | Test weapon
Unknown                    | Unknow
Unsmashed                  | Unsmashed
Vehicle box                | Vehicle box
Vehicle bvh                | Vehicle bvh
Vehicle not bvh            | Vehicle not bvh

# Material

## Setup

:pushpin: Note: Allways Export/Save ur Shaders throu GIMS to speed up ur workflow.
 
# Shader

## Clouds
 
*Parameter set:*

   clouds_altitude

   clouds_anim

   clouds_animsoft

   clouds_fast

   clouds_fog

   clouds_soft

## Vehicle
    
*Parameter set:*
   
## Glass
 
*Parameter set:*

   glass

   glass_breakable

   glass_breakable_screendooralpha

   glass_displacement

   glass_emissive

   glass_emissive_alpha

   glass_emissivenight

   glass_emissvenight_alpha

   glass_env

   glass_normal_spec_reflect

   glass_pv

   glass_pv_env

   glass_reflect

   glass_spec
   
## Parallax
 
*Parameter set:*
   
## Cloth
 
*Parameter set:*
   
## Ped
 
*Parameter set:*
   
## Water
 
*Parameter set:*
   
## Terrain
 
*Parameter set:*
   
## Trees
 
*Parameter set:*
   
## Weapon
 
*Parameter set:*
   
## Decal
 
*Parameter set:*

   decal

   decal_amb_only

   decal_diff_only_um

   decal_dirt

   decal_emissive_only

   decal_emissivenight_only

   decal_glue

   decal_normal_only

   decal_shadow_only

   decal_spec_only

   decal_tnt

   mirror_decal

   normal_decal

   normal_decal_pxm

   normal_decal_pxm_tnt

   normal_reflect_decal

   normal_spec_decal

   normal_spec_decal_detail

   normal_spec_decal_nopuddle

   normal_spec_decal_pxm

   normal_spec_decal_tnt

   normal_spec_detail_dpm_vertdecal_tnt

   normal_spec_reflect_decal

   reflect_decal

   spec_decal

   spec_reflect_decal
   
## Emissive
 
*Parameter set:*

   emissive

   emissive_additive_alpha

   emissive_additive_uv_alpha

   emissive_alpha

   emissive_alpha_tnt

   emissive_clip

   emissive_speclum

   emissive_tnt

   emissivenight

   emissivenight_alpha

   emissivenight_geomnightonly

   emissivestrong

   emissivestrong_alpha

   normal_spec_emissive

   normal_spec_reflect_emissivenight

   normal_spec_reflect_emissivenight_alpha
   
## Mirror
 
*Parameter set:*
   
## Cutout
 
*Parameter set:*

   cutout

   cutout_fence

   cutout_fence_normal

   cutout_hard
   
## Normal Bump
 
*Parameter set:*

   gta_normal

   normal

   normal_alpha
   
## Reflect
 
 *Parameter set:*
   
## Specular
 
*Parameter set:*

   default_spec

   gta_spec

   spec

   spec_alpha

   spec_const

   spec_screendooralpha

   spec_tnt

   spec_twiddle_tnt
 
## Default
 
*Parameter set:*

   custom_default

   default
   
      Diffuse Texture
      Hard Alpha
      Use tessellation
      
   *Add Parameter:*
   
      GlobalAnimUV0
      GlobalAnimUV1
      WetnessMultiplier
      matMaterialColorScale

   default_detail

   default_noedge

   default_tnt

   default_um
   
      Diffuse Texture
      Hard Alpha
      Use tesselation
      Global umParams: ScaleH/ScaleV/FreqH/FreqV  
      
   *Add Parameter:*
   
      matMaterialColorScale
      umGlobalOverrideParams0

   gta_default
   
## Other
 
*Parameter set:*

# Textures

## Basics

   *Size*

      4x4, 64x64, 128x128, 256x256, 512x512, 1024x1024 additional any combination of these sizes

   *File formats*

      dds, png

   *Pixel formats*

      DTX5

      DTX3

      DTX1

      A8R8G8B8

## Embeded Textures

## External Textures

# Integration

## Replacement

## DLC

### Definition files

### File structure

### Encryption
