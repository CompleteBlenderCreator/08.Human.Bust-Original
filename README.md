# Complete Blender Creator - Section 8 - Human Bust

This is the [Complete Blender Creator course]( http://gdev.tv/cbcgithub) - one of the bestselling and highest rated Blender courses on Udemy! Continually updated in response to student suggestions, you will benefit from the fact we have already taught over 360,336 students game development and design, many shipping commercial games as a result.

You're welcome to download, fork or do whatever else legal with all the files! The real value is in our huge, high-quality online tutorials that accompany this repo. You can check out the course here: [Complete Blender Creator]( http://gdev.tv/cbcgithub)

## In This Section

### Section 8 Introduction ###

Michael Introduces The Human Head Section

Focus On 2 Main Topics
+ Mesh topology.
+ Material creation.

### Section 8 Reference Material ###

+ Drawn or photos are both OK.
+ They’re going to define your model. 
+ Guide and Influence your character. 
+ Just following along or without reference material will lead to frustration and a lot of wasted time.
+ Drawn or photos are both OK.
+ They’re going to define your model. 
+ Guide and Influence your character. 
+ Just following along or without reference material will lead to frustration and a lot of wasted time.

### Good Mesh Topology ###

+ 2 Objects can have the same shape, yet a different mesh construction.
+ Use quads wherever possible. nGons and Triangles will cause pinching in your model.
+ Topology can determine how easy it is to edit or animate an object.
+ Topology defines a faces key shapes.
+ Edge/Face loops will follow features.
+ Loops will help with editing.
+ Loops will help with deformation / animation.

### Possible Construction Methods ###

+ Box Modelling: Building up the model from a primitive, adding detail as we go.
+ Poly to Poly: Building up your model one polygon at a time.
+ Sculpting and then Re-Topologising: Can be very time consuming

### Introduction To Retopology ###

+ You have probably already done it to some degree.
+ Remaking a mesh so that the arrangement of polygons is uniform and often all quads.
+ Can significantly lower the polygon count.
+ Planning can help avoid doing much of it.
+ Start low LOD and working up can help avoid it too.
+ It is time consuming.

**Do you Need to Retopologise?**

+ Almost always.
+ Planning can help avoid it.
+ If sculpting the original model it will be necessary.
+ Leads to a clean and well defined mesh.
+ Others can then work with your mesh too.
+ It enables animation possibilities.
+ Allows you to refine and easily edit your mesh.

### Creating The Base Mesh ###

+ You can Add Images as planes, this allows you to see the image all the time in the viewport.
+ Adding images as background images will only show the images when looking Top/bottom, Left/Right, Front Back and in orthographic view.
+ Create a base Mesh to start with and SaveAs when you reach a point where you can branch to make different models.

### The Grease Pencil ###

+ Making notes on your model.
+ Sketching and planning ideas.
+ Roughing out Shapes
+ Converted to edges
+ It can be use to create 2D Animations

### The Knife Tool ###

+ You'll learn how to use the knife tool.
+ See that it gives you many opportunities to craft and re-craft your model.
+ Understand that it can both ruin and fix your topology.

### Rip and Rip Fill ###

+ You'll learn how to use the Rip tool.
+ You’ll learn how to use the Rip Fill tool too!
+ Useful when you wish to add detail that otherwise would be difficult or time consuming to construct.

### Vertex Slide and Edge Slide ###

+ You'll learn about edge and vertex sliding.
+ See that it is a useful way of refining your model without having to create or remove existing geometry.

### Routing Face Loops Using Poles ###

+ You'll learn more about where poles are really useful.
+ How to use a pole to terminate edge/face loops.
+ How they can guide and redirect edge/face loops.
+ Remember a edge/face loop doesn’t have to link back to itself.

### Defining A Face's Main Face Loops ###

+ Define the 5 main face groups that make up the face.
+ Expect to make mistakes. Go with it and remember to Save often, and be prepared to start over from the base head.
+ Create the Nose

### Getting The Right Skin Tone ###

+ There aren’t any right settings
+ Skin is a complex surface.
+ It has more than one tone.
+ It’s shiny in some places, dry in others
+ Skin can be thin or thick letting some light through or blocking it all.

### 3 Point Lighting ###

+ My Scene Contains no direct lighting as of yet.
+ Lighting can change the feel and look of a scene.
+ A lot can be learnt from photo/videography.
+ When using Cycles lighting should be setup as it would be in the real world for best results.
+ 3 point lighting is a common lighting method.
+ 3 Lights: Key Light, Fill Light and Backlight.

### Subsurface Scattering ###

+ Light penetrates the surface of an object
+ Scattered in the material
+ Some light leaves the surface at a different point.
+ The more distance the light travels before exiting, the more it will be absorbed
+ Thicker areas will absorb more than thinner ones.
+ Most shaders we have used so far are direct surface scattering

### The Layer Weight Node ###

+ Usually used for controlling the weighting of shaders via the mix shader node.
+ The Fresnel output has a very sharp fall off.
+ The Facing output blends from one shader to the other more linearly.
+ Both depend on the angle of incidence of the surface in relation to the viewer/camera.

### Physics Based Rendering (PBR) ###

+ Render Time PBR is necessary for creating anything realistic.
+ Getting something looking like it does in the real world is critical to a lot of work.
+ Cycles is almost there, but is misses a few points
+ It doesn’t calculate Fresnel automatically and roughness can be tweaked to be more useable.

### The Color Ramp Node ###

+ The ColorRamp node is used for mapping values to colours with the use of a gradient.
+ It can be customised to produce interesting results.
+ We will be using it to control a single value so can stick with Grey scale.
+ Used to graphically control values.

### How Light Interacts With A Surface ###

+ Gain a better understanding of how light works in the real world and how that transfers into cycles.
+ Look at 6 ways that light and surfaces interact.
+ Gain some understanding about the physics behind how our materials are working.
+ We’re not going to get too deep into the math behind it!

### The Fresnel Node ###

+ Makes things more physically accurate.
+ Everything has a fresnel effect in the real world
+ Cycles doesn’t do it by default.
+ Low Roughness > High amount of Fresnel
+ High Roughness > Low amount of Fresnel

### Reusing Shaders And Materials ###

+ No longer will you have to keep making the same basic shaders again and again.
+ You’ll learn how to start your own library of shaders and materials.
+ Gives you the ability to continually improve your shaders and materials.

### The MixRGB Node ###

+ We’ll use it to mix 2 colours together.
+ See that it can be used to mix more that just colours together.
+ It accepts 6 channels in through 2 colour inputs and 3 channels out- mixing together the 2 colour inputs together based up a Blend type and factor.

### The Geometry Node ###

+ Use this node to take control of an object's normals.
+ You’ll see the vector coordinates we will observe are represented as WORLD Space normals
+ We shall use this node to control the amount of fresnel based upon the amount of roughness.

### Hue Saturation Value (HSV) ###

+ We’ll get to grips with what Hue Saturation and Value mean.
+ A HSV Value is a cylindrical representation of a point in RGB colour space.
+ Hue simply means colour/shade.
+ Saturation is how much there is of that colour.
+ Value can be considered like brightness.

### Making Objects Separately ###

+ We’re getting back to modelling.
+ We cannot fully texture our model until the modelling stage is complete.
+ We’ll take a look at the ear. - With all the folds it can be a challenge!
+ There are 2 main loops for the ear, the inner and outer one.
+ We’re going to make it separately in order to focus on the model.
+ Isolation can be a good and bad thing.

### Joining Separate Objects ###

+ We will join the 2 meshes together forming one mesh object
+ There is more than one way to do this.
+ It is likely to involve some re-topology.

### Adding Detail with Sculpting ###

+ We’ll see that detail can be added in various ways
+ Use the multiresolution modifier to create derived data.
+ Sculpt the rest of the facial detail we need.

**Other Options?**

+ Manually move the vertices about.
+ Add more vertices (ill advised)
+ An accomplished artist could potentially paint the detail straight away.

### UV Unwrapping A Head ###

+ Think about your seams.
+ Try and leave the face intact -without seams.
+ Discover any parts that need their own island

### Texturing The Head ###

+ We’ll make sure our seams are in the right place.
+ Connect our texture to the model.
+ Test to make sure it is working as expected

### Reviewing Your Work Objectively ###

+ We will take an objective look at our model and see what is missing.
+ First : Any Improvements to modelling
+ Second: Any improvements that need to be made to texturing.
+ Finally: Lighting and Environment

### Section 8 Wrap Up ###
