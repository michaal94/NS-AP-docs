---
layout: default
title: Setup
nav_order: 2
has_children: true
---

# Setup

[Git-lfs](https://git-lfs.github.com/) is required for correct cloning of the repository due to scene `.blend` file being over 100MB. 

To setup NS-AP please visit and clone the [repository](https://github.com/michaal94/NS-AP):
```bash
git clone https://github.com/michaal94/NS-AP.git
cd NS-AP
```
Or if using SSH authorisation:
```bash
git clone git@github.com:michaal94/NS-AP.git
cd NS-AP
```

We suggest using docker or conda environment to use NS-AP. The main requirements of NS-AP are:
- Python 3.7.4
- Blender 2.83.20
- [robosuite](https://github.com/ARISE-Initiative/robosuite)

When using Blender the exact version of Python is necessary for the pipeline to work. Additionally, external python instance has to be linked to Blender. Also, we change certain files inside robosuite (we are currently working towards aleviating this necessity).

We noticed memory issuses on some machines using docker. If that happens to you, please consider using conda environment.