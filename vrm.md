## About creating VRM

### What is VRM?

>General-purpose standard for 3D avatars "VRM (Virtual Railroad Models)"
>It was announced by Dwango Co., Ltd. in April 2018.

>VRM extends the general purpose 3D format "glTF 2.0" developed by the Khronos group
>This format is optimized for VR software and VTuber distribution.

><font color="Blue">By limiting it to humanoids, we maintain high compatibility with software that handles avatars.</font>

>* Khronos is a technology consortium of non-profit organizations that develop 3D technologies such as "OpenGL" and "Vulkan".


### How can I make a VRM?

>There are two methods.
>・ Create with modeling software that supports VRM storage (VRoidStudio, etc.)
>-Save the created model in FBX, modify it in Unity, adjust it, and then convert it to VRM.

>The latter is after downloading and installing Unity
>Download the VRM assets and add them to Unity.

><font color="Blue">When you are ready, take in the created model data (FBX etc.), make adjustments, and make adjustments.
>It is basically exported to VRM, but the difficulty is not low.</font>

>Recently, it seems that the number of modeling software that supports it is gradually increasing.

>Free modeling software Blender with additional plugins
>VRM import is possible.
>When creating a VRM, output it with FBX and convert it to VRM with Unity.

>Also, the modeling software MAYA used by professionals
>There is a plugin that supports VRM export.
>* VRM import is not supported.


### What are the precautions when creating a VRM for use with 3tene?

>Here are some points to note when creating a VRM.

>#### About VRM created by VRoidStudio

>It's okay to load a VRM created in VRoidStudio with 3tene,
>When you import a VRM created by VRoidStudio into unity
><font color="Blue">The set value of the eye bone will change, and the range of movement of the eye will be narrowed.
>Eye modifications are required before exporting to VRM.</font>

>Also, if drawing collapse occurs in some clothes, 3tene
>Try changing the quality to "Very High" or higher on the Settings "System" tab.
>![image](image/quality_vroid.png "quality")


>#### About First Person

>Since 3tene supports VR, VRM must support First Person.
>If it is not supported, the phenomenon that the eyes, eyelids, and mouth are displayed twice will occur.

>Make the VRM compatible with First Person or apply it to the relevant facial area
>Disable First Person by changing the setting to "Third Person Only".
><font color="Blue">* If First Person is disabled, problems will occur in drawing when using VR.</font>

>#### Automatic facial expression change for iPhoneX face tracking (facial expression recognition)

>If you create your own facial expression with reference to [this](#ft_iphone_expression.md)
>It is possible to prevent conflict of mouth movements.


### What are the VRM specifications?

>You can get assets for Unity and refer to technical specifications from the following site.

>VRM official website
>Japanese: <a href="https://vrm.dev/" target="_blank">https://vrm.dev/</a>
>English: <a href="https://vrm.dev/en/" target="_blank">https://vrm.dev/en/</a>

>VRM technical specifications (differences from glTF 2.0 and extended specifications)
><a href="https://github.com/vrm-c/vrm-specification/blob/master/specification/0.0/README.ja.md" target="_blank">Japanese</a>　<a href="https://github.com/vrm-c/vrm-specification/blob/master/specification/0.0/README.md" target="_blank">English</a>
