# HoloLens Unity Seed Project

 - Unity Version: __Unity 2019.3.15f1__.
 - Mixed Reality Toolkit Version: __MRTK 2.4.0__.
 - Mixed Reality Curriculum: https://aka.ms/MixedRealityCurriculum
 - Introduction to Mixed Reality with Unity: https://aka.ms/UnityIntroToMixedReality
 - Mixed Reality Curriculum Youtube Playlist: https://aka.ms/MixedRealityCurriculumVideos.

- [Overview](#overview)
- [What's New](#whats-new)
- [Setting up your project](#setup)
- [How to update your project to latest seed](#how-to-update-your-project-to-latest-seed)

## Overview



You can use this repo to get started with [HoloLens development](https://docs.microsoft.com/windows/mixed-reality/?WT.mc_id=aiml-0000-ayyonet) with [Unity 3D](https://docs.microsoft.com/windows/mixed-reality/unity-development-overview?WT.mc_id=aiml-0000-ayyonet). You can download this repo and open the folder with Unity or clone the git repo by following the [setup steps](#setup) below.

Seed project already has the latest [Mixed Reality Toolkit v2](https://docs.microsoft.com/windows/mixed-reality/mrtk-getting-started?WT.mc_id=aiml-0000-ayyonet) added as an asset. Unused assets will not be included in Unity build. If you prefer to not have the assets, you can delete them anytime.

You can get started with  [Mixed Reality Toolkit v2](https://docs.microsoft.com/windows/mixed-reality/mrtk-getting-started?WT.mc_id=aiml-0000-ayyonet) example seens, under Assets > MixedRealityToolkit.Examples > Demos > ... > Scenes.

![Mixed Reality Toolkit Example Scenes](Assets/Images/MRTKAssetsScenes.png)

Find the latest [MRTK release notes here](https://microsoft.github.io/MixedRealityToolkit-Unity/version/releases/2.3.0/Documentation/Updating.html#updating-220-to-230?WT.mc_id=hololensseedproject-github-ayyonet).

<a href="http://www.youtube.com/watch?feature=player_embedded&v=8FBLNoeUSvk" target="_blank"><img src="http://img.youtube.com/vi/8FBLNoeUSvk/0.jpg" 
alt="Mixed Reality Toolkit version 2.2.0 feature video" width="854" height="480" border="10"/></a>

## What's New?

* Initial support for Unity 2019.3 and the XR SDK architecture.
* Centralized dependencies folder (when using MSBuild for Unity).
* Hand physics service.

![Hand physics service](Assets/Images/mrtkCollision.gif)

* Non-native keyboard (Experimental).

![Non-native keyboard (Experimental)](Assets/Images/mrtkKeyboard.png)

* Hand coach (Experimental).

![Hand coach (Experimental)](Assets/Images/mrtkHand.png)

* Follow solver (Experimental).
A solver that matches HoloLens 2 shell behavior.

![Hand coach (Experimental)](Assets/Images/mrtkFollow.gif)

* ObjectManipulator and BoundsControl (Experimental).

![Hand coach (Experimental)](Assets/Images/mrtkBoundsCtrl.gif)

## Setup

You can clone and delete this repository's history and start a new git project by running the below script. You need to create your own github repo first. Replace <your-project-name> with your own github project url. 

```git
git clone --depth=1 https://github.com/Yonet/HoloLensUnitySeedProject.git <your-project-name>
```

OR 
```git

// Clone the seed project
git clone --depth=1 https://github.com/Yonet/HoloLensUnitySeedProject.git

-- Remove the history from the repo
rm -rf .git

-- recreate the repos from the current content only
git init
git add .
git commit -m "Initial commit"

-- push to the github remote repos ensuring you overwrite history
git remote add origin git@github.com:<YOUR ACCOUNT>/<YOUR REPOS>.git
git push -u --force origin master

```
## How to update your project to latest seed?

Whenever there is a new update for  [Mixed Reality Toolkit](https://microsoft.github.io/MixedRealityToolkit-Unity/README.html?WT.mc_id=hololensseedproject-github-ayyonet) or [Azure Spatial Anchors](https://docs.microsoft.com/azure/spatial-anchors/?WT.mc_id=aiml-0000-ayyonet) packages, this repo will be updated with the latest version. You can automaticly get the latest packages by adding the seed repo as your upstream and pulling from it. 

```
git remote add upstream https://github.com/Yonet/HoloLensUnitySeedProject.git
git pull upstream master
```

You can check to see if your remote origin and upstream by running:

```
git remote -v
```

You can remove the upstream anytime by running:

```
git remote remove upstream https://github.com/Yonet/HoloLensUnitySeedProject.git
``` 
