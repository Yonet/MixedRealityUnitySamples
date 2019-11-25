# Mixed Reality Unity Samples

## Overview

You can use this repo to get started with [HoloLens development](https://docs.microsoft.com/windows/mixed-reality/?WT.mc_id=hololensseedproject-github-ayyonet) with [Unity 3D](https://docs.microsoft.com/windows/mixed-reality/unity-development-overview?WT.mc_id=hololensseedproject-github-ayyonet). You can download this repo and open the folder with Unity or clone the git repo by following the steps below. 

Seed project already has the latest [Mixed Reality Toolkit v2](https://docs.microsoft.com/windows/mixed-reality/mrtk-getting-started?WT.mc_id=hololensseedproject-github-ayyonet) added as an asset. Unused assets will not be included in Unity build. If you prefer to not have the assets, you can delete them anytime. 

This repo is following the [HoloLens 2 Unity Tutorial](https://docs.microsoft.com/en-us/windows/mixed-reality/mrlearning-base?WT.mc_id=hololensseedproject-github-ayyonet). You can find the steps in different branches of the repo and the master brach will have the finished version. 

## Steps

 - [Master branch](https://github.com/Yonet/HoloLensUnitySeedProject/tree/master)
 - [Step-1 branch](https://github.com/Yonet/HoloLensUnitySeedProject/tree/step-1): [Initializing your project and first application](https://docs.microsoft.com/en-us/windows/mixed-reality/mrlearning-base-ch1?WT.mc_id=hololensseedproject-github-ayyonet)

## Setup

You can clone and delete this repository's history and start a new git project by running the below script. You need to create your own github repo first. Replace <your-project-name> with your own github project url. 

```git
git clone --depth=1 https://github.com/Yonet/HoloLensUnitySeedProject.git <your-project-name>
```

OR 
```git

// Clone the seed project
git clone --depth=1 https://github.com/Yonet/HoloLensUnitySeedProject.git

-- Remove the history from 
rm -rf .git

-- recreate the repos from the current content only
git init
git add .
git commit -m "Initial commit"

-- push to the github remote repos ensuring you overwrite history
git remote add origin git@github.com:<YOUR ACCOUNT>/<YOUR REPOS>.git
git push -u --force origin master

```
