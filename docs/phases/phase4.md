# Phase 4: Allow Complex Styling in Notes (1 day)

## Rails
### Models
* Review

### Controllers
* ReviewsController (create, update, destroy)

### Views
* workspaces/show.json.jbuilder
* reviews/index.json.jbuilder

## Flux
### Views (React Components)
* Workspace Item
  - Workspace Information
    - Gallery
    - Hours
    - Ratings
    - Extra Business Info
  - Reviews Index
    - Review Form
    - Reviews Index Item

### Stores
* Review

### Actions
* ApiActions.receiveOneWorkspace
* ApiActions.receiveAllReviews

### ApiUtil
* ApiUtil.fetchOneWorkspace
* ApiUtil.fetchAllReviews
* ApiUtil.createReview
* ApiUtil.editReview
* ApiUtil.deleteReview

## Gems/Libraries
* Twitter Bootstrap
