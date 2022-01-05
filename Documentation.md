# GTA5-Model-Documentation

# Index
[**Basics**](./Documentation.md#basics)
- [Programs](./Documentation.md#programs)
   - [System](./Documenation.md#system)
   - [Models](./Documenation.md#models)
   - [Textures](./Documentation.md#textures)
   - [Minimap](./Documentation.md#minimap)

[**Data file types**](./Documentation.md#data-file-types)
- [RPF](./Documentation.md#rpf) 
- [Ytype](./Documentation.md#ytype)
- [Ydr](./Documentation.md#ydr)
- [Ybn](./Documentation.md#ybn)
- [Ytd](./Documentation.md#ytd)
- [Ymap](./Documentation.md#ymap)
- [Xml](./Documentation.md#xml)

[**Model**](./Documentation.md#model)
- [Basics](./Documentation.md#basics-1)
- [Create](./Documentation.md#create)
- [Import](./Documentation.md#import)
- [Export](./Documentation.md#export)

[**Collision**](./Documentation.md#collision)
- [Collision types](./Documentation.md#collision-types)
   - [Embeded Collision](./Documentation.md#embeded-collision)
   - [Static Collision](./Documentation.md#static-collision)
- [Collision Flaggs](./Documentation.md#collision-flaggs)

[**Material**](./Documentation.md#material)
- [Setup](./Documentation.md#setup)
- [Material list](./Documentation.md#material-list)
   - [Hard terrain](./Documentation.md#hard-terrain)
   - [Loose terrain](./Documentation.md#loose-terrain)
   - [Vegetation](./Documentation.md#vegetation)
   - [Metals](./Documentation.md#metals)
   - [Woods](./Documentation.md#woods)
   - [Manmade](./Documentation.md#manmade)
   - [Glass](./Documentation.md#glass)
   - [Vehicles](./Documentation.md#vehicles)
   - [Liquids](./Documentation.md#liquids)
   - [Misc](./Documentation.md#misc)
   - [Projtex](./Documentation.md#projtex)
   - [VFX specific particles](./Documentation.md#vfx-specific-particles)
   - [VFX specific explosions](./Documentation.md#vfx-specific-explosions)
   - [Physics](./Documentation.md#physics)
   - [Natrual motion](./Documentation.md#natrual-motion)
   - [New Materials](./Documentation.md#new-materials)

[**Shader**](./Documentation.md#shader)
- [Parameter Description](./Documentation.md#parameter-description)
- [Parameter sets](./Dcomuentation.md#parameter-sets)
   - [Clouds](./Documentation.md#clouds)
   - [Vehicle](./Documentation.md#vehicle-1)
   - [Glass](./Documentation.md#glass-1)
   - [Parallax](./Documentation.md#parallax)
   - [Cloth](./Documentation.md#cloth)
   - [Ped](./Documentation.md#ped)
   - [Water](./Documentation.md#water)
   - [Terrain](./Documentation.md#terrain)
   - [Trees](./Documentation.md#trees)
   - [Weapon](./Documentation.md#weapon)
   - [Decal](./Documentation.md#decal)
   - [Mirror](./Documentation.md#mirror)
   - [Cutout](./Documentation.md#cutout)
   - [Normal Bump](./Documentation.md#normal-bump)
   - [Reflect](./Documentation.md#reflect)
   - [Specular](./Documentation.md#specular)
   - [Default](./Documentation.md#default)
   - [Other](./Documentation.md#other)

[**Textures**](./Documentation.md#textures-1)
- [Basics](./Documentation.md#basics-2)
   - [Size](./Documentation.md#size)
   - [File formats](./Documentation.md#file-formats)
   - [Pixel formats](./Documentation.md#pixel-formats)
- [Embeded Textures](./Documentation.md#embeded-textures)
- [External Textures](./Documentation.md#external-textures)

[**Minimap**](./Documentation.md#minimap-1)
- [Export](./Documentation.md#export-1)
- [Edit](./Documentation.md#edit)
- [Import](./Documentation.md#import-1)

[**Integration**](./Documentation.md#integration)
- [Replacement](./Documentation.md#replacement)
- [DLC](./Documentation.md#dlc)
   - [Definition files](./Documentation.md#definition-files)
   - [File structure](./Documentation.md#file-structure)
   - [Encryption](./Documentation.md#encryption)

# Basics

## Programs

### System

GTA 5

[OpenV](https://openiv.com/)

[CodeWalker](https://github.com/dexyfex/CodeWalker/)

[Archive Fix](https://gtaforums.com/topic/871168-affix-fix-your-rpf-archives-and-work-without-openiv/)

### Models

[Autodesk 3ds Max](https://www.autodesk.de/products/3ds-max/overview)

*Addonscript Autodesk*   
[GIMS Evo](https://de.gta5-mods.com/tools/gims-evo-with-gta-v-support/)

[Blender](https://www.blender.org/)

*Pythonscript* 
[Openformat-to-obj](https://github.com/hedgehog90/openformat-to-obj/)

### Textures

[Krita](https://krita.org/en/)

[Awesomebump](https://github.com/kmkolasinski/AwesomeBump/)

### Minimap

[GFX Editor](https://github.com/jindrapetrik/jpexs-decompiler/releases)

# Data file types

## Rpf

Archivefile, wich can contains different datafiles. Existing RPF can be deactivated throu content.xml in an dlc.

## Ytype

Asset definition file with case sensitive xml syntax which providing additional data for the system like draw boundings,
physics directorie and more.

***Assettypes***
>
>   **Drawable**
>
>   Defintion of an object base on a ydr model.
>
>   **Milo**
>
>   Definition of zones and models to load. It uses Entity definition to build an array, 
>   which is be used to set items to zones.
>
>   **Entity**
>
>   Definition of objects which are used in Milo.

## Ydr

   Model file

## Ybn

   Static collision file is an additional model to an existing one. It contains mostly 
   simple box collisions which matches the geometry of its parent model.

## Ytd

   Texturedictionary file

## Ymap

   Map position definition file

## Xml

   System definition file contains data in xml which are directly handled by the system. 
   These files are case sensetive in its structure.

# Model

## Basics

   Normal direction

   Vertexcount

   Material

   Meshmodifier

## Create

## Import

*to GTA5*

*to Autodesk 3ds*

## Export

*from GTA5*

*from Autodesk 3ds*

# Collision

## Collision types

Collision FX are definend within the Material

### Embeded Collision

On map load it will be loaded last, blocks flags only. Maximum allowed vertecies +32k.

### Static Collision

On map loading it will be loaded first, blocks rain and snow automaticly.

## Collision Flaggs

Flags 1                    | Flags 2 
------------               | -------------
Defines group of collision | Defines group of collision to interact with
Animal                     | Animal
Animal Ragdoll             | Animal Ragdoll
Explosion                  | Exlosion
Foliage                    | Foliage
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

A list of materials can be found in the game files *material.dat* which is be used by Gims Evo.
Materials in Autodesk 3ds must be named like the material in material.dat u want to use, else
the Gims Evo converts the material to default.

## Setup

:pushpin: ***Note:*** Allways Export/Save ur Shaders throu GIMS to speed up ur workflow.
 
## Material list

### Hard Terrain
   
CONCRETE             
CONCRETE_POTHOLE        
CONCRETE_DUSTY          
TARMAC                  
TARMAC_PAINTED          
TARMAC_POTHOLE          
RUMBLE_STRIP            
BREEZE_BLOCK            
ROCK                 
ROCK_MOSSY              
STONE                
COBBLESTONE             
BRICK                
MARBLE                  
PAVING_SLAB             
SANDSTONE_SOLID            
SANDSTONE_BRITTLE 

### Loose Terrain

SAND_LOOSE  
SAND_COMPACT    
SAND_WET    
SAND_TRACK  
SAND_UNDERWATER   
SAND_DRY_DEEP  
SAND_WET_DEEP  

ICE   
ICE_TARMAC  
SNOW_LOOSE  
SNOW_COMPACT    
SNOW_DEEP   
SNOW_TARMAC 

GRAVEL_SMALL   
GRAVEL_LARGE   
GRAVEL_DEEP       
GRAVEL_TRAIN_TRACK   
DIRT_TRACK  
MUD_HARD       
MUD_POTHOLE      
MUD_SOFT       
MUD_UNDERWATER       
MUD_DEEP         
MARSH       
MARSH_DEEP        
SOIL  
CLAY_HARD   
CLAY_SOFT      

### Vegetation

GRASS_LONG  
GRASS    
GRASS_SHORT       
HAY   
BUSHES   
TWIGS 
LEAVES   
WOODCHIPS   
TREE_BARK   

### Metals

METAL_SOLID_SMALL       
METAL_SOLID_MEDIUM           
METAL_SOLID_LARGE       
METAL_HOLLOW_SMALL       
METAL_HOLLOW_MEDIUM        
METAL_HOLLOW_LARGE   
METAL_CHAINLINK_SMALL   
METAL_CHAINLINK_LARGE   
METAL_CORRUGATED_IRON   
METAL_GRILLE   
METAL_RAILING  
METAL_DUCT  
METAL_GARAGE_DOOR       
METAL_MANHOLE  

### Woods

WOOD_SOLID_SMALL     
WOOD_SOLID_MEDIUM       
WOOD_SOLID_LARGE     
WOOD_SOLID_POLISHED       
WOOD_FLOOR_DUSTY        
WOOD_HOLLOW_SMALL       
WOOD_HOLLOW_MEDIUM         
WOOD_HOLLOW_LARGE       
WOOD_CHIPBOARD          
WOOD_OLD_CREAKY            
WOOD_HIGH_DENSITY       
WOOD_LATTICE         

### Manmade

CERAMIC  
ROOF_TILE        
ROOF_FELT         
FIBREGLASS        
TARPAULIN         
PLASTIC        
PLASTIC_HOLLOW          
PLASTIC_HIGH_DENSITY       
PLASTIC_CLEAR           
PLASTIC_HOLLOW_CLEAR       
PLASTIC_HIGH_DENSITY_CLEAR       

FIBREGLASS_HOLLOW       
RUBBER         
RUBBER_HOLLOW        
LINOLEUM          
LAMINATE       
CARPET_SOLID         
CARPET_SOLID_DUSTY           
CARPET_FLOORBOARD       
CLOTH          
PLASTER_SOLID        
PLASTER_BRITTLE           
CARDBOARD_SHEET         
CARDBOARD_BOX        
PAPER       
FOAM        
FEATHER_PILLOW       
POLYSTYRENE          
LEATHER        
TVSCREEN          
SLATTED_BLINDS       

### Glass

GLASS_SHOOT_THROUGH        
GLASS_BULLETPROOF       
GLASS_OPAQUE         

PERSPEX     

### Vehicles

CAR_METAL               
CAR_PLASTIC             
CAR_SOFTTOP               
CAR_SOFTTOP_CLEAR          

CAR_GLASS_WEAK 
CAR_GLASS_MEDIUM  
CAR_GLASS_STRONG  
CAR_GLASS_BULLETPROOF   
CAR_GLASS_OPAQUE  

### Liquids

WATER 
BLOOD 
OIL   
PETROL   

### Misc

FRESH_MEAT  
DRIED_MEAT  

### Projtex

EMISSIVE_GLASS             
EMISSIVE_PLASTIC  

### VFX specific particles

VFX_METAL_ELECTRIFIED   
VFX_METAL_WATER_TOWER   

### VFX specific explosions

VFX_METAL_STEAM   
VFX_METAL_FLAME

### Physics

*USE FOR BOWLING LANES SO THE SCRIPT HAS TOTAL CONTROL OVER THE BOWLING BALL MOVEMENT*                                                                      
PHYS_NO_FRICTION  

*USED FOR BALL IN THE GOLF MINI-GAME SO THAT IT CAN BE TWEAKED WITHOUT AFFECTING OTHER OBJECTS IN THE WORLD*                                                                        
PHYS_GOLF_BALL 

*USED FOR BALL IN THE TENNIS MINI-GAME SO THAT IT CAN BE TWEAKED WITHOUT AFFECTING OTHER OBJECTS IN THE WORLD*                                                                         
PHYS_TENNIS_BALL  

*USED FOR CASTERS ON TROLLEYS TO MAKE IT SLIDE AROUND THE FLOOR*                                                                                      
PHYS_CASTER    

*USED FOR CASTERS ON TROLLEYS TO MAKE IT SLIDE AROUND THE FLOOR - HIGHER FRICTION VERSION*                                                                                       
PHYS_CASTER_RUSTY    

*USED ON VEHICLES OVER AREA WHERE A DOOR OR WINDOW CAN FALL OFF - IT KEEPS THE CONVEX HULL REQUIREMENTS FOR THE COLLISION*                                                                
PHYS_CAR_VOID           

*SET ONLY IN CODE FOR THE MAIN NON RAGDOLL PED CAPSULE*                                                                                               
PHYS_PED_CAPSULE        

*MATERIALS THAT THE PHYSICS NEEDS CAUSE A REACTION TO*                                                                                 
PHYS_ELECTRIC_FENCE        
PHYS_ELECTRIC_METAL        
PHYS_BARBED_WIRE        

*MATERIALS FOR THE BILLIARDS MINI GAME*                                                                                          
PHYS_POOLTABLE_SURFACE     
PHYS_POOLTABLE_CUSHION     
PHYS_POOLTABLE_BALL  

### Natrual motion

BUTTOCKS    
THIGH_LEFT     
SHIN_LEFT   
FOOT_LEFT   
THIGH_RIGHT    
SHIN_RIGHT     
FOOT_RIGHT     
SPINE0      
SPINE1   
SPINE2   
SPINE3   
CLAVICLE_LEFT     
UPPER_ARM_LEFT          
LOWER_ARM_LEFT          
HAND_LEFT         
CLAVICLE_RIGHT       
UPPER_ARM_RIGHT   
LOWER_ARM_RIGHT   
HAND_RIGHT     
NECK     
HEAD     

ANIMAL_DEFAULT    

### New materials

CAR_ENGINE  
PUDDLE   
CONCRETE_PAVEMENT    
BRICK_PAVEMENT    

*SPECIAL MATERIAL USED TO IDENTIFY FRAG BOUNDS USED ONLY FOR COVER SHAPE TESTS AND DISABLED WHEN THE FRAG BREAKS*          
PHYS_DYNAMIC_COVER_BOUND      

VFX_WOOD_BEER_BARREL    
WOOD_HIGH_FRICTION      

*SPECIAL VERSIONS OF THESE MATERIAL THAT WONT HAVE PLANT INSTANCE PLACEMENT ON THEM - IDEALLY THESE NEED REPLACED WITH A MATERIAL FLAG GOING FORWARD*          
ROCK_NOINST       

BUSHES_NOINST     
METAL_SOLID_ROAD_SURFACE      

# Shader

## Parameter Description

***Diffuse Texture***
.
.
.

## Parameter Sets

### Clouds

**clouds_altitude**

**clouds_anim**

**clouds_animsoft**

**clouds_fast**

**clouds_fog**

**clouds_soft**

### Vehicle
    
*Parameter set:*
   
### Glass
 
**glass**
> Bump Texture
> 
> Diffuse Texture
>
> Enviorment Texture(Cube)
>
> Bumpiness
>
> Reflectivity
>
> Specular Falloff
>
> Specular Fresnel
>
> Specular Intensity
>
> Use tessellation

**glass_breakable**
> Bump Texture
>
> Diffuse Texture
>
> Specular Texture
>
> BrokenDiffuseColor
>
> BrokenSpecularColor
>
> Bumpiness
>
> DecalTint
>
> specular map intensity mask color
>
> Specular Falloff
>
> Specular Fresnel
>
> Specular Intensitiy
>
> Use tessellation
>
> ***Additional Parameter***
>
> CrackDecalBumpAlphaThreshold
>
> CrackDecalBumpAmout
>
> CrackDecalBumpTileScale
>
> CrackEdgeBumpAmount
>
> CrackEdgeBumpTileScale

**glass_breakable_screendooralpha**
> Bump Texture
>
> Diffuse Texture
>
> Specular Texture
>
> BrokenDiffuseColor
> 
> BrokenSpecularColor
>
> Bumpiness
>
> DecalTint
>
> specular map intensity mask color
>
> Specular Falloff
>
> Specular Fresnel
>
> Specular Intensity
>
> Use tessellation
>
> ***Additional Parameter***
>
> CrackDecalBumpAlphaThreshold
>
> CrackDecalBumpAmout
>
> CrackDecalBumpTileScale
>
> CrackEdgeBumpAmount
>
> CrackEdgeBumpTileScale

**glass_displacement**
> Bump Texture
>
> Diffuse Texture
>
> Enviorment Texture (Cube)
>
> Specular Texture
>
> Bumpiness
>
> Reflectivity
>
> specular map intensity mask color
>
> Specular Falloff
>
> Specular Fresnel
>
> Specular Intensity
>
> Use tessellation
>
> Displacement: scaleU,scaleV,camDist

**glass_emissive**
> Bump Texture
>
> Diffuse Texture
>
> Enviorment Texture (Cube)
>
> Bumpiness
>
> Emissive HDR Multiplier
>
> Reflectivity
>
> Specular Falloff
>
> Specular Fresnel
>
> Specular Intensity
> 
> Use tessellation
>
> ***Additional Parameters***
>
> GlobalAnimUV0
>
> GlobalAnimUV1

**glass_emissive_alpha**
> Bump Texture
>
> Diffuse Texture
>
> Enviorment Texture (Cube)
>
> Bumpiness
>
> Emissive HDR Multiplier
>
> Reflectivity
>
> Specular Falloff
> 
> Specular Fresnel
>
> Specular Intensity
>
> Use tessellation
>
> ***Additional Parameter***
> 
> GlobalAnimUV0
>
> GlobalAnimUV1

**glass_emissivenight**
> Bump Texture
>
> Diffuse Texture
>
> Enviorment Texture (Cube)
>
> Bumpiness
>
> Emissive HDR Multiplier
>
> Reflectivity
>
> Specular Falloff
>
> Specular Fresnel
>
> Specular Intensity
>
> Use tessellation

**glass_emissvenight_alpha**
> Bump Texture
> 
> Diffuse Texture
>
> Enviorment Texture (Cube)
>
> Bumpiness
>
> Emissive HDR Multiplier
>
> Reflectivity
>
> Specular Falloff
>
> Specular Fresnel
>
> Specular Intensity
>
> Use tessellation

**glass_env**
> Bump Texture
>
> Diffuse Texture
>
> Specular Texture
>
> Bumpiness
>
> specular map intensity mask color
>
> Specular Falloff
>
> Specular Fresnel
>
> Specular Intensity
>
> Use tessellation
>
> ***Additional Parameter***
>
> GlobalAnimUV0
>
> GlobalAnimUV1

**glass_normal_spec_reflect**
> Bump Texture
>
> Diffuse Texture
>
> Enviorment Texture (Cube)
>
> Specular Texture
>
> Bumpiness
>
> Reflectivity
>
> specular map intensity mask color
>
> Specular Falloff
>
> Specular Fresnel
>
> Specular Intensity
>
> Use tessellation

**glass_pv**
> Diffuse Texture
> 
> BrokenDiffuseColor
>
> BrokenSpecularColor
>
> Crack Decal Bump Alpha Threshold
>
> DecalTint
>
> Specular Falloff
>
> Specular Fresnel
>
> Specular Intensity
>
> Use tessellation
>
> ***Additional Parameter***
>
> CrackDecalBumpAmount
>
> CrackDecalBumpTileScale
>
> CrackEdgeBumpAmount
>
> CrackEdgeBumpTileScale

**glass_pv_env**
> Diffuse Texture
>
> BrokenDiffuseColor
>
> BrokenSpecularColor
>
> Crack Decal Bump Alpha Threshold
>
> DecalTint
>
> Specular Falloff
>
> Specular Fresnel
>
> Specular Intensity
>
> Use tessellation
> 
> ***Additional Parameter***
>
> CrackDecalBumpAmount
>
> CrackDecalBumpTileScale
>
> CrackEdgeBumpAmount
>
> CrackEdgeBumpTileScale

**glass_reflect**
> Diffuse Texture
>
> Enviorment Texture (Cube)
>
> Reflectivity
>
> Specular Falloff
>
> Specular Fresnel
>
> Specular Intensity
>
> Use tessellation

**glass_spec**
> Diffuse Texture
>
> Specular Texture
>
> specular map intensity mask color
>
> Specular Falloff
>
> Specular Fresnel
> 
> Specular Intensity
>
> Use tessellation
   
### Parallax
 
*Parameter set:*
   
### Cloth
 
*Parameter set:*
   
### Ped
 
*Parameter set:*
   
### Water
 
*Parameter set:*
   
### Terrain
 
*Parameter set:*
   
### Trees
 
*Parameter set:*
   
### Weapon
 
*Parameter set:*
   
### Decal
 
**decal**
> Diffuse Texture
>
> Specular Falloff
> 
> Specular Fresnel
>
> Specular Intensity
>
> Use tessellation
>
> ***Additional Parameter***
> 
> WetnessMultiplier

**decal_amb_only**
> Diffuse Texture
>
> ambient map mask color
>
> Use tessellation
>
> ***Additional Parameter***
>
> matMaterialColorScale

**decal_diff_only_um**
> Diffuse Texture
>
> Use tessellation
> 
> Global umParams:ScaleH/ScaleV/FreqH/FreqV
>
> ***Additional Parameter***
> 
> WetnessMultiplier
>
> matMaterialColorScale
>
> umGlobalOverrideParams0

**decal_dirt**
> Diffuse Texture
>
> dirt map mask color
>
> Specular Falloff
>
> Specular Fresnel
>
> Specular Intensity
>
> Use tessellation

**decal_emissive_only**
> Diffuse Texture
>
> Emissive HDR Multiplier
>
> Use tessellation
>
> ***Additional Parameter***
>
> matMaterialColorScale

**decal_emissivenight_only**
> Diffuse Texture
>
> Emissive HDR Multiplier
>
> Use tessellation
>
> ***Additional Parameter***
>
> matMaterialColorScale

**decal_glue**
> Diffuse Texture
>
> Specular Falloff
> 
> Specular Fresnel
>
> Specular Intensity
>
> Use tessellation

**decal_normal_only**
> Bump Texture
>
> Diffuse Texture
>
> Bumpiness
>
> Specular Falloff
>
> Specular Fresnel
>
> Specular Intensity
>
> Use tessellation

**decal_shadow_only**
> Diffuse Texture
>
> Use tessellation
> 
> ***Additional Parameter***
>
> matMaterialColorScale

**decal_spec_only**
> Diffuse Texture
>
> Specular Texture
>
> specular map intensity mask color
>
> Specular Falloff
>
> Specular Fresnel
>
> Specular Intensity
>
> Use tessellation

**decal_tnt**
> Diffuse Texture
>
> Tint Palette
>
> Specular Falloff
>
> Specular Fresnel
>
> Specular Intensity
>
> Tint Palette Selector
>
> Use tessellation
> 
> ***Additional Paramerter***
>
> WetnessMultiplier

**mirror_decal**
> Bump Texture
>
> Diffuse Texture
>
> Bumpiness
>
> Reflectivity
>
> Specular Fresnel
>
> Use tessellation
>
> Distorion Amount
>
> ***Additional Parameter***
>
> gMirrorBounds

**normal_decal**
> Bump Texture
>
> Diffuse Texture
>
> Bumpiness
>
> Specular Falloff
>
> Specular Fresnel
>
> Specular Intensity
>
> Use tessellation
>
> ***Additional Parameter***
>
> GlobalAnmiUV0
>
> GlobalAnimUV1
>
> WetnessMultiplier

**normal_decal_pxm**
> Bump Texture
>
> Diffuse Texture
>
> Height Texture
>
> Bumpiness
>
> Height Bias
>
> Heigth Scale
>
> Parallax Self Shadow
>
> Specular Falloff
>
> Specular Fresnel
>
> Specular Intensity
>
> Use tessellation
>
> ***Additional Parameter***
>
> GlobalAnimUV0
>
> GlobalAnimUV1
>
> WetnessMultiplier

**normal_decal_pxm_tnt**
> Bump Texture
>
> Diffuse Texture
>
> Height Texture
>
> Tint Palette
>
> Bumpintess
>
> Height Bias
>
> Height Scale
>
> Parallax Self Shadow
>
> Specular Falloff
>
> Specular Fresnel
>
> Specular Intensity
>
> Tint Palette Selector
>
> Use tessellation

**normal_decal_tnt**
> Bump Texture
>
> Diffuse Texture
>
> Tint Palette
>
> Bumpiness
>
> Specular Falloff
>
> Specular Fresnel
>
> Specular Intensity
>
> Tint Palette Selector
>
> Use tessellation

**normal_reflect_decal**
> Bump Texture
>
> Diffuse Texture
>
> Enviorment Texture (Cube)
>
> Bumpiness
>
> Reflectivity
>
> Use tessellation

**normal_spec_decal**
> Bump Texture
>
> Diffuse Texture
>
> Specular Texture
>
> Bumpiness
>
> specular map intensity mask color
>
> Specular Falloff
>
> Specular Fresnel
>
> Specular Intensity
>
> Use tessellation
>
> ***Additional Parameter***
>
> GlobalAnimUV0
>
> GlobalAnimUV1
>
> WetnessMultiplier

**normal_spec_decal_detail**
> Bump Texture
>
> Detail Map
>
> Diffuse Texture
>
> Specular Texture
>
> Bumpiness
>
> detail Inten Bump Scale
>
> specular map intensity mask color
>
> Specular Falloff
>
> Specular Fresnel
>
> Specular Intensity
>
> Use tessellation

**normal_spec_decal_nopuddle**
> Bump Texture
>
> Diffuse Texture
>
> Specular Texture
>
> Bumpiness
>
> specular map intensity mask color
>
> Specular Falloff
>
> Specular Fresnel
>
> Specular Intensity
>
> Use tessellation
>
> ***Additional Parameter***
>
> WetnessMultiplier

**normal_spec_decal_pxm**
> Bump Texture
>
> Diffuse Texture
>
> Height Texture
>
> Specular Texture
>
> Bumpiness
>
> Height Bias
>
> Height Scale
>
> Parallax Self Shadow
>
> specular map intensity mask color
>
> Specular Falloff
>
> Specular Fresnel
>
> Specular Intensity
>
> Use tessellation
>
> ***Additional Parameter***
>
> GlobalAnimUV0
> 
> GlobalAnimUV1
>
> WetnessMultiplier

**normal_spec_decal_tnt**
> Bump Texture
>
> Diffuse Texture
>
> Specular Texture
>
> Tint Palette
>
> Bumpiness
>
> specular map intensity mask color
>
> Specular Falloff
>
> Specular Fresnel
>
> Specular Intensity
>
> Tint Palette Selector
>
> Use tessellation
>
> ***Additional Parameter***
>
> WetnessMultiplier

**normal_spec_detail_dpm_vertdecal_tnt**
> Bump Texture
>
> Detail Map
>
> Diffuse Texture
>
> Secondary Texture
>
> Height Texture
>
> Specular Texture
>
> Tint Palette
>
> Bumpiness
>
> detail Inten Bump Scale
>
> Hard Alpha
>
> Height Bias
>
> Height Scale
>
> specular map intensity mask color
>
> Specular Falloff
>
> Specular Fresnel
>
> Specular Intensity
>
> Tessellation Mul
>
> Tint Palette Selector
>
> UseTessellation
>
> ***Additional Parameter***
>
> WetnessMultiplier

**normal_spec_reflect_decal**
> Bump Texture
>
> Diffuse Texture
>
> Environment Texture (Cube)
>
> Specular Texture
>
> Bumpiness
>
> Reflectivity
>
> specular map intensity mask color
>
> Specular Falloff
>
> Specular Fresnel
>
> Specular Intensity
>
> Use tessellation

**reflect_decal**
> Diffuse Texture
>
> Environment Texture (Cube)
>
> Reflectivity
>
> Use tessellation

**spec_decal**
> Diffuse Texture
>
> Specular Texture
>
> specular map intensity mask color
>
> Specular Falloff
>
> Specular Fresnel
>
> Specular Intensity
>
> Use tessellation

**spec_reflect_decal**
> Diffuse Texture
>
> Environment Texture (Cube)
>
> Specular Texture
>
> Reflectivity
>
> specular map intensity mask color
>
> Specular Falloff
>
> Specular Fresnel
>
> Specular Intensity
>
> Use tessellation
   
### Emissive

**emissive**
> Diffuse Texture
>
> Emissive HDR Multiplier
>
> Hard Alpha
>
> Use tessellation
>
> ***Additional Parameter***
>
> GlobalAnimUV0
>
> GlobalAnimUV1
>
> natNaterialColorScale

**emissive_additive_alpha**
> Diffuse Texture
>
> Emissive HDR Multiplier
>
> Use tessellation
>
> ***Additional Parameter***
>
> matMaterialColorScale

**emissive_additive_uv_alpha**
> Diffuse Texture
>
> Emissive HDR Multiplier
>
> Use tessellation
>
> ***Additional Parameter***
>
> GlobalAnimUV0
>
> GlobalAnimUV1
>
> matMaterialColorScale

**emissive_alpha**
> Diffuse Texture
>
> Emissive HDR Multiplier
>
> Hard Alpha
>
> Use tessellation
>
> ***Additional Parameter***
>
> GlobalAnimUV0
>
> GlobalAnimUV1
>
> matMaterialColorScale

**emissive_alpha_tnt**
> Diffuse Texture
>
> Tint Palette
>
> Emissive HDR Multiplier
>
> Hard Alpha
>
> Tint Palette Selector
>
> Use tessellation
>
> ***Additional Parameter***
>
> matMaterialColorScale

**emissive_clip**
> Diffuse Texture
>
> Emissive HDR Multiplier
>
> Hard Alpha
>
> Use tessellation
>
> ***Additional Parameter***
>
> GlobalAnimUV0
>
> GlobalAnimUV1
>
> matMaterialColorScale

**emissive_speclum**
> Diffuse Texture
>
> Emissive HDR Multiplier
>
> Hard Alpha
>
> Specular Falloff
>
> Specular Fresnel
>
> Specular Intensity
>
> Use tessellation
>
> ***Additional Parameter***
>
> matMaterialColorScale

**emissive_tnt**
> Diffuse Texture
>
> Tint Palette
>
> Emissive HDR Multiplier
>
> Hard Alpha
>
> Tint Palette Selector
>
> Use tessellation
>
> ***Additional Parameter***
>
> matMaterialColorScale

**emissivenight**
> Diffuse Texture
>
> Emissive HDR Multiplier
>
> Hard Alpha
>
> Use tessellation
>
> ***Additional Parameter***
>
> matMaterialColorScale

**emissivenight_alpha**
> Diffuse Texture
>
> Emissive HDR Multiplier
>
> Hard Alpha
>
> Use tessellation
>
> ***Additional Parameter***
>
> matMaterialColorScale

**emissivenight_geomnightonly**
> Diffuse Texture
>
> Emissive HDR Multiplier
>
> Hard Alpha
>
> Use tessellation
>
> ***Additional Parameter***
>
> matMaterialColorScale

**emissivestrong**
> Diffuse Texture
>
> Emissive HDR Multiplier
>
> Hard Alpha
>
> Use tessellation
>
> ***Additional Parameter***
>
> GlobalAnimUV0
>
> GlobalAnimUV1
>
> matMaterialColorScale

**emissivestrong_alpha**
> Diffuse Texture
>
> Emissive HDR Multiplier
>
> Hard Alpha
>
> Use tessellation
>
> ***Additional Parameter***
>
> GlobalAnimUV0
>
> GlobalAnimUV1
>
> matMaterialColorScale

**normal_spec_emissive**
> Bump Texture
>
> Diffuse Texture
>
> Specular Texture
>
> Bumpiness
>
> Emissive HDR Multiplier
>
> Hard Alpha
>
> specular map intensity mask color
>
> Specular Falloff
>
> Specular Fresnel
>
> Specular Intenstity
>
> Use tessellation

**normal_spec_reflect_emissivenight**
> Bump Texture
>
> Diffuse Texture
>
> Specular Texture
>
> Bumpiness
>
> Emissive HDR Multiplier
>
> specular map intensity mask color
>
> Specular Falloff
>
> Specular Fresnel
>
> Specular intenstity
>
> Use tessellation

**normal_spec_reflect_emissivenight_alpha**
> Bump Texture
>
> Diffuse Texture
>
> Specular Texture
>
> Bumpiness
>
> Emissive HDR Multiplier
>
> specular map intensity mask color
>
> Specular Falloff
>
> Specular Fresnel
>
> Specular intenstity
>
> Use tessellation

### Mirror
 
*Parameter set:*
   
### Cutout

**cutout**

**cutout_fence**

**cutout_fence_normal**

**cutout_hard**
   
### Normal Bump

**gta_normal**

**normal**
> Bump Texture
>
> Diffuse Texture
>
> Bumpiness
>
> Specular Intensity
>
> Specular Falloff
>
> Specular Fresnel
>
> Hard Alpha
>
> Use tessellation
>
>***Additional Parameter***
>   
> GlobalAnimUV0
>
> GlobalAnimUV1
>
> WetnessMultiplier
>
> matMaterialColorScale

**normal_alpha**
   
### Reflect
 
 *Parameter set:*
   
### Specular

**default_spec**

**gta_spec**

**spec**

**spec_alpha**

**spec_const**

**spec_screendooralpha**

**spec_tnt**

**spec_twiddle_tnt**
 
### Default

**custom_default**

**default**
> Diffuse Texture
>
> Hard Alpha
>
> Use tessellation
>  
>***Additional Parameter:***
>   
> GlobalAnimUV0
>
> GlobalAnimUV1
>
> WetnessMultiplier
>
> matMaterialColorScale

**default_detail**

**default_noedge**

**default_tnt**

**default_um**  
> Diffuse Texture
>
> Hard Alpha
>
> Use tesselation
>
> Global umParams: ScaleH/ScaleV/FreqH/FreqV  
>    
>***Additional Parameter:***
>   
> matMaterialColorScale
>
> umGlobalOverrideParams0

**gta_default**
   
### Other
 
*Parameter set:*

# Textures

## Basics

### Size

4x4, 64x64, 128x128, 256x256, 512x512, 1024x1024 additional any combination of these sizes

### File formats

dds, png

### Pixel formats

DTX5

DTX3

DTX1

A8R8G8B8

## Embeded Textures

## External Textures

# Minimap

## Export

## Edit

## Import

# Integration

## Replacement

## DLC

### Definition files

### File structure

### Encryption
