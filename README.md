# GH Workflows

Common Repo for Github Workflows and Actions

## Goal

This should be a common repo for at least all Passport apps.

## Current State

1. This hosts the build workflow for the main Passport repo
2. Scorer workflows have been somewhat modified to run in a similar style, but
   not completely.
3. Scorer staging and production workflows should be made to match each other
4. Alternative Python Test and Dockerize actions can be added to this repo,
   protected by IF statements. These should be the only differences for
   passport vs. scorer
5. Scorer can switch to use this repo
6. Staking can likely integrate this repo as-is for the frontend.
   Need to add a flag for the backend build so it can be skipped
