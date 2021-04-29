# To integrate hyper & trajectory into other mods

## please keep in mind that

hyper & trajectory requires **OXCE** to run.
it would not work on OXC version, because it uses **refNode** and

    vapor(Color/Density/Probability)Surface

flag, which is OXCE specific.

## Step 1: metadata modification

add the following code to end of the metadata.yml.

    resourceConfig: transparency.rul

it would look like this:

    name: "Mod Name"
    version: "version number"
    description: "descriptionn"
    author: "author"
    id: "mod-id"
    master: "xcom1"
    resourceConfig: transparency.rul

## Step 2: adding required files

hyper & trajectory consists of three ruleset files:

- hypervelocity.rul
- trajectories.rul
- transparency.rul

to integrate ruleset files:

- put _hypervelocity_ and _trajectories_ into **Ruleset** folder (or any other folder)
- put transparency.rul file into the same hierarchy as **metadataa.yml**
