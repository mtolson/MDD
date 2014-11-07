# Deployment Process

##New Feature Branch
* Checkout Master
 * git checkout master
* Create a New Feature Branch
 * git branch deploymentBranch
 * git checkout deploymentBranch
*Make changes/add/remove files/code
*Add & Commit changes to New Feature Branch
 * git add -A
 * git commit -m "Message about commit"


## Merge Branch or Branches into Deployment Branch
* Checkout Master
 * git checkout master
* Create a deployment Branch
 * git branch deploymentBranch
 * git checkout deploymentBranch
* Merge Branch or Branches into a Deployment Branch
 * git merge newFeatureBranch
* Resolve any conflicts


##Staging
* Push deploymentBranch branch to staging server
 * git push StagingServer master
* QA Site and ensure everything is correct
 * If issue is found create a new branch and fix issue
 * Merge fix with depolymentBranch
 * Push to Staging, retest
* Have others/clients review site and get the ok for Production push

##Production
* Checkout Master
 * git checkout master
* Merge deploymentBranch into Master
 * git merge deploymentBranch
* Push master branch to Production server
 * git push LiveServer master
* Push master to github
 * git push github master
* QA and ensure everything is working correctly
 * If issue is found then create a Hotfix
 
##Hotfix
* Checkout Master
 * git checkout master
* Create a Hotfix Branch
 * git branch hotfix branch
 * git checkout hotfix
* Fix issue
 * git add -A
 * git commit -m "Message about commit" 
* Merge with Master
 * git checkout master
 * git merge deploymentBranch
* Push to Production Server
 * git push LiveServer master
* Push master to github
 * git push github master



