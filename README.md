 # Horizon Pool Tutorial

**This is a very early draft. Comments and constructive criticism are very welcome!**

Since one of the major stumbling block for new users is the extension Horizon's pool, this tutorial aims to give a step-by-step guide on how to create new parts. It will focus on the basics at first to get you started as fast as possible and cover the most important cases, but also later introduce more advanced concepts needed for more peculiar parts.

This tutorial is meant to be beginner-friendly. If you come across any steps which are not immediately clear to you, please raise the issue. Lack of clarity is definitively a bug and has to be fixed!

Screenshots and procedures in this tutorial are from Horizon 1.1. The general structure of the pool is not likely to change but some details might. If some inconsistencies to the current version become apparent, please leave a note so this tutorial can be updated.

## Outline

Of course, the devil is in the details and trying to fit all different aspects and tips and gotchas into one tutorial might be possible, but it'd be a pretty long tutorial. To keep it manageable, this tutorial is actually several, where each one focuses on some detail of the process. To keep it hands on, each of the chapters will add a new part, from start to finish (well, except for the introductory chapter).

Since I'll submit PRs to the pool for the parts created here to help the pool progress, they will probably already be in the pool once you read this guide. Nevertheless, I'd encourage you to follow along and experiment a bit instead of just reading the tutorial and trying to take everything in.

### [Chapter 1: Introduction](01_introduction.md)

This chapter gives some background on why the pool is the way it is and strives to make the basic structure clear. No part is added to the pool here, but we'll browse around and try to find our way.

### Chapter 2: Included pools, pool set-up for contributions

After some specific details on how the pool is sub-divided internally, we can look at it as a whole. This chapter deals with included pools and their use in projects, but also with the general workflow of contributions to the pool.

### Chapter 3: Basic part creation

A first part! This chapter covers the most basic case, when most of what we need is already in the pool and we just need to tie the ends together to make a new part. We'll create a LM324 quad op-amp from existing symbols and packages and submit a pull request to the main pool repository.

### Chapter 4: Drawing symbols

Say our design calls for a small signal JFET, the J111, which isn't in the pool so far. Enough variants of the TO-92 package already exist, but there is no symbol yet. This chapter will get you acquainted with text placements and orientations, so the symbol will look good in every case.

### Chapter 5: Expandable symbols, alternative pin names and the footprint generator

We'd like to see the ATSAMD11D14A, a neat little microcontroller, in the pool. The footprint generator can help with the package, but we'll have to draw the symbol on our own. We'll have a look at alternative pin names and what it means to mark a symbol as expandable.

### Chapter 6: Custom padstacks

This chapter uses the NVTFS5C478NL, a n-Channel MOSFET with a particularly weird pad shape, as an example for adding a custom padstack and drawing a package without the help of the package generator.

### Chapter 7: Cutouts, keepouts, and alternative packages

TBD

### Chapter 8: Scripted part creation and parametric data

TBD

## Further readings

The first place to go is of course the [official documentation](https://horizon-eda.readthedocs.io/en/latest/), which is continually improved. Particularly relevant for our endeavours is the [Horizon pool convention](https://github.com/horizon-eda/horizon-pool-convention), which lists general rules for all parts in the pool. It's of course a bit more dry than a tutorial like this and while not a required reading for this guide (the relevant rules are repeated here as we go along), you should probably have a look once you want to submit your own parts to the pool.

