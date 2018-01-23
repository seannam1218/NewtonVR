## Summary

**Now available on the Unity Asset store: [https://www.assetstore.unity3d.com/en/#!/content/75712](https://www.assetstore.unity3d.com/en/#!/content/75712)**

**Go to [newtonvr.readme.io](http://newtonvr.readme.io) for documentation, guides on how to get started with NewtonVR, and basic integration instructions.**

**Our feature roadmap is public and can be found on Trello here: [https://trello.com/b/iLvugNpK/newtonvr](https://trello.com/b/iLvugNpK/newtonvr)**

Our system allows players to pick up, drop, throw, and use held objects. Items don't pass through other items (rigidbodies), or the environment (non-rigidbodies). Rather, held items interact with other rigidbodies naturally -- taking mass into account. For example, if you have two boxes of the same mass they can push each other equally, but a balloon, with considerably less mass, can't push a box.

*For more information on this style of mass-based interaction, [see this article by Nick Abel](http://www.vrinflux.com/newton-vr-physics-based-interaction-on-the-vive/), one of the creators of NewtonVR.*
<img class='gfyitem' data-id='DistantPitifulAfricanhornbill' />

Items can be configured to be picked up at any point, or when grabbed, can rotate and position themselves to match a predefined orientation. This lets you pick up a box from its corner as well as pick up a gun and have it orient to the grip.
<img class='gfyitem' data-id='ImpureTautBergerpicard' />

We've also created a few physical UI elements to help with basic configuration and "menu type scenarios. We also give you the option to dynamically let the controllers turn into physical objects on a button press.
<img class='gfyitem' data-id='PointlessImperturbableBorzoi' />

<br>
NewtonVR brought to you by [Tomorrow Today Labs](http://www.tomorrowtodaylabs.com):

**Development:** Keith Bradner, Nick Abel<br>**Interaction Design:** Adrienne Hunter<br>**Modeling:** Wesley Eldridge, Carli Wood<br>**Audio:** Joshua Du Chene

## Notes about Mixed Reality support (Experimental)

[@Jesseric](https://twitter.com/jerressic) and I ([@meulta](https://twitter.com/meulta)) added the support for [Windows Mixed Reality](https://developer.microsoft.com/en-us/windows/mixed-reality). 

Steps to use it:
- You don't have to change anything and your newtonVR code should work on Mixed Reality headsets and controllers. 
- For now MR only works with the MRTP version of Unity (grab the latest which is 5 today [here](http://beta.unity3d.com/download/a07ad30bae31/download.html))
- Add the Mixed Reality Toolkit to your project as an asset. You can clone it from here: https://github.com/Microsoft/MixedRealityToolkit
- One MRTK is added to the project, open the **Mixed Reality Toolkit** menu and go in **Configure > Apply Mixed Reality Project** Settings. Check **Target Occluded Devices** and click **Apply**
- Check **Enable Windows MR** on the *NVRHand* game object
- Test you app! Controllers meshes are downloaded from drivers so they should match the controllers you are using. Physics should work too.

If you have any question ping me on ([twitter](https://twitter.com/meulta))