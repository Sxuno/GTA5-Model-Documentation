# GTA5-Model-Documentation

# Basics

   Programs

      GTA 5

      OpenV

      CodeWalker

      Archive Fix

      Autodesk 3ds Max

         Addonscript
   
            GIMS Evo

      Blender

      Krita

      Awsomebump



# Data file types

   Rpf

      Archivefile

   Ytype

      Asset definition file

      Assettypes

         Drawable

         Milo

         Entity

   Ydr

      Model file

   Ybn

      Static collision file

   Ytd

      Texturedictionary file

   Ymap

      Map position definition file

   Xml

      System definition file

# Model

   Basics

      Normal direction

      Vertexcount

      Material

      Meshmodifier

   Create

   Export
 
# Collision

   Collision types

      - Embeded Collision

      - Static Collision

   Collision Flaggs

      Flags 1

      Defines group of collision

         - Animal
         - Animal ragdoll
         - Explosion
         - Foliage
         - Forklift forks
         - Glass
         - Map animal
         - Map cover
         - Map deep surface
         - Map dynamic
         - Map river
         - Map stairs
         - Map vehicle
         - Map weapon
         - Object
         - Object env cloth
         - Ped
         - Pickup
         - Plant
         - Projectile
         - Ragdoll
         - Smoke
         - Test ai
         - Test camera
         - Test script
         - Test vehicle wheel
         - Test weapon
         - Unknown
         - Unsmashed
         - Vehicle bok
         - Vehicle bvh
         - Vehicle not bvh

      Flags 2

      Defines group of collision to interact with

         - Animal
         - Animal ragdoll
         - Explosion
         - Foliage
         - Forklift forks
         - Glass
         - Map animal
         - Map cover
         - Map deep surface
         - Map dynamic
         - Map river
         - Map stairs
         - Map vehicle
         - Map weapon
         - Object
         - Object env cloth
         - Ped
         - Pickup
         - Plant
         - Projectile
         - Ragdoll
         - Smoke
         - Test ai
         - Test camera
         - Test script
         - Test vehicle wheel
         - Test weapon
         - Unknown
         - Unsmashed
         - Vehicle bok
         - Vehicle bvh
         - Vehicle not bvh
    
# Material

   Setup
 
# Shader

   Clouds 
 
      Parameter set:

         clouds_altitude

         clouds_anim

         clouds_animsoft

         clouds_fast

         clouds_fog

         clouds_soft

   Vehicle
    
      Parameter set:
   
   Glass
 
      Parameter set:

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
   
   Parallax
 
      Parameter set:
   
   Cloth
 
      Parameter set:
   
   -Ped
 
      Parameter set:
   
   Water
 
      Parameter set:
   
   Terrain
 
      Parameter set:
   
   Trees
 
      Parameter set:
   
   Weapon
 
      Parameter set:
   
   Decal
 
      Parameter set:

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
   
   Emissive
 
      Parameter set:

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
   
   Mirror
 
      Parameter set:
   
   Cutout
 
      Parameter set:

         cutout

         cutout_fence

         cutout_fence_normal

         cutout_hard
   
   Normal Bump
 
      Parameter set:

         gta_normal

         normal

         normal_alpha
   
   Reflect
 
      Parameter set:
   
   Specular
 
      Parameter set:

         default_spec

         gta_spec

         spec

         spec_alpha

         spec_const

         spec_screendooralpha

         spec_tnt

         spec_twiddle_tnt
   
   Default
 
      Parameter set:

         custom_default

         default

            Diffuse Texture

            Hard Alpha

            Use tessellation

               Add Parameter:

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

               Add Parameter:

                  matMaterialColorScale
                  umGlobalOverrideParams0

         gta_default


   
   Other
 
      Parameter set:

# Textures

   Basics

      Size

         4x4, 64x64, 128x128, 256x256, 512x512, 1024x1024 additional any combination of these sizes

      File formats

         dds, png

      Pixel formats

         DTX5

         DTX3

         DTX1

         A8R8G8B8

   Embeded Textures

   External Textures

# Integration

   Replacement

   DLC

      Definition files

      File structure

      Encryption
