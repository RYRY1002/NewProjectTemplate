# NewProjectTemplate
A template for new projects in Unreal Engine 5.

## Installation
### Project Installation
1. Download the project
   - Downloads in the releases page are polished, final releases
   - Download the repository as a .zip or clone it for the most up to date version, but it may have bugs
2. Extract the .zip file
3. Copy the files to wherever you keep your Unreal Engine projects
4. Open Unreal Engine 5.0.0 Preview 2 and open the project
5. Done

### Pre-compiled Shaders Installation
1. Download the pre-compiled shaders from the latest release *(pre-compiled shaders will only be updated with new releases)*
2. Copy/Move the `Common` folder and place it in `C:\Users\<user>\AppData\Local\UnrealEngine`

## Updating existing projects
If you have a project that already uses this template, but you'd like to update it with new master materials and such,

1. Download the new version
2. Go into the `Content` folder and copy whatever you'd like to update.
3. Replace the old files with the new ones.

The shaders will need to recompile (~250 shaders), but once that's done, everything should just work.

## Materials
### Material Layer Assets
All base Material Layer assets can be located in `Game/Materials/_Layers`.

* `MasterBlends/Normal/blend-mask`
  - Uses a mask to blend between layers
* `MasterBlends/Normal/blend-procedural`
  - Uses perlin noise, lerps and height maps to blend between layers
* `MasterLayers/Normal/surface`
  - This layer asset should be used for regular surfaces
  - It supports Albedo, Metallic, Specular, Roughness, Emissive, Normal, AO, POM, and various tiling methods
* `MasterLayers/Normal/surface_additive`
  - This layer asset should be used for things that are added to the scene (such as fire, steam, holograms, etc.)
  - It supports Albedo, Metallic, Specular, Roughness, Emissive, Normal, AO, POM, and various tiling methods
  - Uses additive blend mode
* `MasterLayers/Normal/surface_masked`
  - This layer asset should be used for things that are either transparent or opaque (such as fences, chains, grates, etc.)
  - It supports Albedo, Metallic, Specular, Roughness, Emissive, Normal, AO, POM, Opacity and various tiling methods
  - Uses masked blend mode
* `MasterLayers/Normal/surface_translucent`
  - This layer asset should be used for things that are partially transparent (such as glass panes, bottles, water, etc.)
  - It supports Albedo, Metallic, Specular, Roughness, Emissive, Normal, AO, POM, Opacity and various tiling methods
  - Uses translucent blend mode

* `MasterBlends/VT/blend-mask`
  - Uses a mask to blend between layers
  - Uses virtual textures
* `MasterBlends/VT/blend-procedural`
  - Uses perlin noise, lerps and height maps to blend between layers
  - Uses virtual textures
* `MasterLayers/VT/surface`
  - This layer asset should be used for regular surfaces
  - It supports Albedo, Metallic, Specular, Roughness, Emissive, Normal, AO, POM, and various tiling methods
  - Uses virtual textures
* `MasterLayers/VT/surface_additive`
  - This layer asset should be used for things that are added to the scene (such as fire, steam, holograms, etc.)
  - It supports Albedo, Metallic, Specular, Roughness, Emissive, Normal, AO, POM, and various tiling methods
  - Uses additive blend mode
  - Uses virtual textures
* `MasterLayers/VT/surface_masked`
  - This layer asset should be used for things that are either transparent or opaque (such as fences, chains, grates, etc.)
  - It supports Albedo, Metallic, Specular, Roughness, Emissive, Normal, AO, POM, Opacity and various tiling methods
  - Uses masked blend mode
  - Uses virtual textures
* `MasterLayers/VT/surface_translucent`
  - This layer asset should be used for things that are partially transparent (such as glass panes, bottles, water, etc.)
  - It supports Albedo, Metallic, Specular, Roughness, Emissive, Normal, AO, POM, Opacity and various tiling methods
  - Uses translucent blend mode
  - Uses virtual textures

### Master Materials
Master Materials can be located in `Game/Materials/_MasterMaterials`.

* `Normal/surface_material`
  - This material be used for regular surfaces
  - It supports Albedo, Metallic, Specular, Roughness, Emissive, Normal, AO, POM, and various tiling methods
* `Normal/surface_material_additive`
  - This material asset should be used for things that are added to the scene (such as fire, steam, holograms, etc.)
  - It supports Albedo, Metallic, Specular, Roughness, Emissive, Normal, AO, POM, and various tiling methods
  - Uses additive blend mode
* `Normal/surface_material_masked`
  - This material should be used for things that are either transparent or opaque (such as fences, chains, grates, etc.)
  - It supports Albedo, Metallic, Specular, Roughness, Emissive, Normal, AO, POM, Opacity and various tiling methods
  - Uses masked blend mode
* `Normal/surface_material_translucent`
  - This material should be used for things that are partially transparent (such as glass panes, bottles, water, etc.)
  - It supports Albedo, Metallic, Specular, Roughness, Emissive, Normal, AO, POM, Opacity and various tiling methods
  - Uses translucent blend mode
* `Normal/decal_material`
  - This material should be used for regular decals
  - It supports Albedo, Metallic, Specular, Roughness, Emissive, Normal, Opacity, POM and various tiling methods
* `Normal/decal_material_modulating`
  - This material should be used for decals that are added to the scene, but need shadowing (such as screws, cable ports, braille, etc.)
  - It supports Albedo, Metallic, Specular, Roughness, Emissive, Normal, Opacity, POM and various tiling methods
  - Uses modulate blend mode
* `Normal/decal_material_stain`
  - This material should be used for decals that are stains (such as puddles, dirt, blood, etc.)
  - It supports Albedo, Metallic, Specular, Roughness, Emissive, Normal, Opacity, POM and various tiling methods

* `VT/VT_surface_material`
  - This material should be used for regular surfaces
  - It supports Albedo, Metallic, Specular, Roughness, Emissive, Normal, AO, POM, and various tiling methods
  - Uses virtual textures
* `VT/VT_surface_material_additive`
  - This material should be used for things that are added to the scene (such as fire, steam, holograms, etc.)
  - It supports Albedo, Metallic, Specular, Roughness, Emissive, Normal, AO, POM, and various tiling methods
  - Uses additive blend mode
  - Uses virtual textures
* `VT/VT_surface_material_masked`
  - This material should be used for things that are either transparent or opaque (such as fences, chains, grates, etc.)
  - It supports Albedo, Metallic, Specular, Roughness, Emissive, Normal, AO, POM, Opacity and various tiling methods
  - Uses masked blend mode
  - Uses virtual textures
* `VT/VT_surface_material_translucent`
  - This material should be used for things that are partially transparent (such as glass panes, bottles, water, etc.)
  - It supports Albedo, Metallic, Specular, Roughness, Emissive, Normal, AO, POM, Opacity and various tiling methods
  - Uses translucent blend mode
  - Uses virtual textures
* `VT/VT_decal_material`
  - This material should be used for regular decals
  - It supports Albedo, Metallic, Specular, Roughness, Emissive, Normal, Opacity, POM and various tiling methods
  - Uses virtual textures
* `Normal/decal_material_modulating`
  - This material should be used for decals that are added to the scene, but need shadowing (such as screws, cable ports, braille, etc.)
  - It supports Albedo, Metallic, Specular, Roughness, Emissive, Normal, Opacity, POM and various tiling methods
  - Uses modulate blend mode
  - Uses virtual textures
* `VT/VT_decal_material_stain`
  - This material should be used for decals that are stains (such as puddles, dirt, blood, etc.)
  - It supports Albedo, Metallic, Specular, Roughness, Emissive, Normal, Opacity, POM and various tiling methods
  - Uses virtual textures

### Example Material Instances
Example Material Instances can be located in `Game/Materials/ExampleMaterials`.

* `DayOff-NightOn_LightFunction`
  - Shows an example of a light function taking advantage of the project's Day/Night time cycle
* `layer_example`
  - Shows an example of material layers being used
* `VT_surface_material_example_earth_day`
  - Shows a fully configured Earth intstance
  - Instance of `VT_surface_material`
* `VT_surface_material_example_earth_night`
  - Shows a fully configured Earth instance
  - Instance of `VT_surface_material`
* `VT_surface_material_translucent_example_earth_clouds`
  - Shows a fully configured Earth cloud system
  - Instance of `VT_surface_material_translucent`
* `VT_surface_material_example_jupiter`
  - Shows a fully configured Jupiter instance
  - Instance of `VT_surface_material`
* `VT_surface_material_example_mars`
  - Shows a fully configured Mars instance
  - Instance of `VT_surface_material`
* `VT_surface_material_example_mercury`
  - Shows a fully configured Mercury instance
  - Instance of `VT_surface_material`
* `VT_surface_material_example_moon`
  - Shows a fully configured Moon instance
  - Instance of `VT_surface_material`
* `VT_surface_material_example_neptune`
  - Shows a fully configured Neptune instance
  - Instance of `VT_surface_material`
* `VT_surface_material_example_saturn`
  - Shows a fully configured Saturn instance
  - Instance of `VT_surface_material`
* `VT_surface_material_translucent_example_saturn_rings`
  - Shows a fully configured Saturn Rings instance
  - Instance of `VT_surface_material_translucent`
* `VT_surface_material_example_stars`
  - Shows a fully configured Stars instance
  - Instance of `VT_surface_material`
* `VT_surface_material_example_stars_milky_way`
  - Shows a fully configured Stars with Milky Way instance
  - Instance of `VT_surface_material`
* `VT_surface_material_example_sun`
  - Shows a fully configured Sun instance
  - Instance of `VT_surface_material`
* `VT_surface_material_example_uranus`
  - Shows a fully configured Uranus instance
  - Instance of `VT_surface_material`
* `VT_surface_material_example_venus_surface`
  - Shows a fully configured Venus Surface instance
  - Instance of `VT_surface_material`
* `VT_surface_material_translucent_example_venus_atmosphere`
  - Shows a fully configured Venus Atmosphere instance
  - Instance of `VT_surface_material_translucent`

### Material Functions
Material Functions can be located in `Game/Materials/Functions`.

* `BreakNormalFromHeight`
  - This reverses the effect of the `StoreHeightInNormal` function 
* `CustomUVs`
  - Adds custom tiling options
  - Used in `surface_material`, `decal_material`, `decal_material_stain`, `blend_material_2` and `blend_material_3`
* `MapAdjustments`
  - Adds configuration options
  - Used in `surface_material`, `decal_material` and `decal_material_stain`
* `Opacity`
  - Fix for `surface_material_masked` and `VT_surface_material_masked`
* `POM`
  - Adds Parallax Occlusion Mapping
  - Used in all master materials
* `Rain`
  - Adds a basic rain effect
  - Used in `surface_material`, `blend_material_2` and `blend_material_3`
* `StoreHeightInNormal`
  - Appends the height map to the normal map.
* `StretchingFix`
  - Applys a fix for stretched textures
  - Used in `surface_material`, `decal_material`, `decal_material_stain`, `blend_material_2` and `blend_material_3`
* `StretchingFix-XY`
  - XY specific streching fix
  - Used in `MF_Tiling_StretchingFix`
* `StretchingFix-XZ`
  - XY specific streching fix
  - Used in `MF_Tiling_StretchingFix`
* `StretchingFix-YZ`
  - YZ specific streching fix
  - Used in `MF_Tiling_StretchingFix`
* `Wind`
  - Adds options for Wind
  - Used in `blend_material_2` and `blend_material_3`

### Parameter Collections
Material Parameter Collections can be located in `Game/Materials/ParameterCollections`.

* `SunMoon_Rotations`
  - Contains rotation values for the Sun and Moon
  - Used in `DayOff-NightOn_LightFunction`

### Textures
Textures can be located in `Game/Materials/Textures`.

* `DirtMask` folder
  - Contains Lens Dirt textures
* `Moon` folder
  - Contains Moon texture
* `Placeholders` folder
  - Contains placeholder textures
  - Used in all master materials

### Post Process Materials
Post Process Materials can be located in `Game/Materials/PostProcess` 

* `Fisheye`
  - Basic fisheye effect
  - Used in `Game/Player/Blueprints/PlayerCharacter.uasset` whilst in Third Person

### UI Materials
UI Materials can be located in `Game/Materials/UI`

* `FisheyeUI`
  - Same basic fisheye effect as in `Game/Player/Materials/Fisheye.uasset` but converted to work with UIs
  - Used in `Game/Player/UI/Physics_WidgetHUD.uasset`

## Blueprints
Blueprints can be located in `Game/Blueprints`.

### DayNightCycle folder
* `DayNightManager`
  - Gives other assets vital information about the Day/Night cycle
* `Moon`
  - Fake Moon

### Spline_Movement folder
* `Spline_Movement_Template`
  - Actor to be moved along the spline defined in `Spline_Movement_Track`
* `Spline_Movement_Track`
  - Defines the track that `Spline_Movement_Template` will move along

### WeatherSystem folder
* `WeatherManager`
  - Controls weather across various assets

### Example folder
* `DayNightLight`
  - Light that turns on at night, and off during the day.
  - Light contains various performance optimizations.
* `Earth+Lighting`
  - Spinning Earth + Lighting
* `SolarSystem`
  - Spinning + Orbiting solar system

## Level
Levels can be located in the main `Game` directory.

* `Empty`
  - As the name suggests, this level is empty.
* `Level`
  - This is the main level.
* `MainMenu`
  - This is the level featured in the main menu. It's the one with the sky.

### World Partition Grids
* `Landscape`
  - Used for landscapes and buildings
* `Actors`
  - Used for large actors (such as streetlamps, shipping containers, etc)
* `SmallActors`
  - Used for small actors (such as trashbags, rubbish decals, etc)

## Day/Night cycle system
The day/night cycle is controlled via the level blueprint and `DayNightManger`.

The level blueprint is what actually rotates the directional lights, `DayNightManager` tells other actors whether it is day or night. (This is useful for example with streetlamps. By accessing the Boolean in `DayNightManager`, the streetlamp can be turned on and off depending on whether it is day or night).

### Examples of Day/Night cycle system

An example of such a streetlight is provided in `Game/Blueprints/Examples/DayNightLight.uasset`. (When placing this blueprint, make sure to select the `DayNightManager` from the details panel)

Another example of the Day/Night cycle system in use is the `DayOff-NightOn_LightFunction` file found in `Game/Materials/ExampleMaterials`.

## Particles
Particles can be located in `Game/Content/Particles`.

## Player
### Player controls

* Mouse Movement - Look Around
* WASD - Movement
* V - Change Camera
* Left Click whilst looking at actor with Physics - Picks up actor
* Right Click whilst looking at actor with Physics - Pokes actor
* Left Click whilst holding an actor with Physics - Drops actor
* Right Click whilst holding an actor with Physics - Throws actor
* R - Turn Ray Tracing On/Off
* Esc - Pause
* P - Pause

### UI
The HUD that the player sees can be configured by opening `Game/Player/UI/PhysicsUI.uasset`.

The HUD uses the Inverted Fisheye effect, so if you want to disable that, just click on the retainer box and set the effect material to nothing.

Additional things can be configured by opening `Game/Player/UI/UI.uasset`.

### Menus
The menus can be found in `Game/Player/UI/MainMenu`, `Game/Player/UI/PauseMenu`, and `Game/Player/UI/LoadingScreen` respectively.

All of the code inside the menus is extremely simple, and should not require explaining.

## Project Settings
### Rendering

* Uses Ray Traced GI
  - 2 Max bounces
  - 6 Samples per pixel
* Uses Ray Traced Reflections
  - 4 Max bounces
  - 1 Sample per pixel
* Uses Ray Traced Shadows
  - Sun and Moon cast shadows with 5 samples per pixel, everything else has 1 sample per pixel.