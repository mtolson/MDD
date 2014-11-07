# Deployment Process

## Merge Branch or Branches into Master
* Merge Branch or Branches into a Deployment Branch
* Resolve any conflicts
* Pull Master From Production
* Merge Master and deployment branch
* Resolve any conflicts

##Staging
* Push master branch to staging server
* QA Site and ensure everything is correct
 * If issue is found create a new branch and fix issue
 * Merge fix with Master
 * Push to Staging, retest
* Have others/clients review site and get the ok for Production push

##Production
* Push master branch to Production server
* Push master to github
* QA and ensure everything is working correctly
 * If issue is found then create a Hotfix
 
##Hotfix
* Create a new branch off of Master
* Fix issue
* Merge with Master
* Push to Production Server