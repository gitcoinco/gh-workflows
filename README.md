# GH Workflows

Common Repo for Github Workflows and Actions

## Goal

This should be a common repo for at least all Passport apps.

## Current State

1. This hosts the build workflow for the main Passport repo
2. Scorer workflows have been somewhat modified to run in a similar style, but
   not completely.
3. Scorer staging and production workflows should be made to match each other
   (i.e. this repo uses the exact same action for the staging and production 
   workflow steps, scorer does not. Also scorer unnecessarily repeats tests
   and dockerizing)
5. Alternative Python Test and Dockerize actions can be added to this repo,
   protected by IF statements. These should be the only differences for
   passport vs. scorer. Some vars may need to be adjusted (e.g. passing in
   the name of the pulumi stack to load when pushing to AWS)
      Note: We may want to look at alternatives, but should head in the general
      direction of sharing actions where it makes sense
5. Scorer can switch to use this repo
6. Staking can likely integrate this repo pretty much as-is for the frontend.
   Need to add a flag for the backend build so it can be skipped
