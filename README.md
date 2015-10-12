# Workspace

[Heroku link][heroku] **NB:** This should be a link to your production site

[heroku]: http://www.herokuapp.com

## Minimum Viable Product

Workspace (gowork.space) is a web application that assists those who work best in a free and out-of-the-office kind of an environment through informed peer reviews regarding workspaces and cafes. Workspace will be built usingh Ruby on Rails and ReactJS. Workspace allows users to:

<!-- This is a Markdown checklist. Use it to keep track of your progress! -->

- [ ] Create an account
- [ ] Log in / Log out
- [ ] Search for workspaces by name and by location
- [ ] Filter their search based on preferences for wifi, price, open now, etc.
- [ ] Look at a workspace / cafe's information, including the reviews
- [ ] Write reviews and upload pictures pertaining to a workspace

## Design Docs
* [View Wireframes][view]
* [DB schema][schema]

[view]: ./docs/views.md
[schema]: ./docs/schema.md

## Implementation Timeline

### Phase 1: Heroku Setup, User Authentication, JSON API (1.5 days)

In this phase, I will first become more comfortable with pushing my code to Heroku and
understanding how to point it to my actual domain site. I will focus on building
the user authentication and have forms for signing in and signing up. The log out
process will be available. It will be styled up nicely with some Twitter Bootstrap.

[Details][phase-one]

### Phase 2: Beginning Flux, App Component, Workspace CRUD, Search Component (2.5 days)

In this phase, I will focus on beginning the setup for the Flux, the React Router,
and the React view structure. My first React view will be the App component, which
will contain the logo, a SearchBar component, and a UserInfo component. For now,
the SearchBar component will be static. If I have time towards the end, I will focus
making this more dynamic and making search more user friendly. After the App view is
complete, I will begin working on the Workspace CRUD. I will seed the database with
some of my favorite workspaces. Then, I will create React views for the Workspace
`Index` and `IndexItem` and the Filter component. At the end of this phase, users
can search for workspace based off its name and location. After they search, a list
of matching results will show as well as the filter options bar. By clicking on the
filter options, the listings will auto refresh. Again, there will be some basic
Twitter Bootstrap styling. Will show up to 10 listings, and users can click next to see more.

[Details][phase-two]

### Phase 3: Google Maps (1.5 days)

In this phase, I will focus on the Map component of the Workspace React view. I
will need to get more familiar with the Google Maps geocode API so that I can plot
the addresses onto the map. At the end of this phase, users can search and see the results on the Google map.

[Details][phase-three]

### Phase 4: Reviews CRUD, Workspace Item Component  (3 days)

The purpose of this phase is when users click on a link pertaining to a workspace. First, I will generate the CRUD for Reviews. The Workspace Item component will contain both the Workspace Information and the Reviews Index components. The Workspace Information component will contain the gallery of pictures and basic business information.The Reviews Index will contain the Review Form, Review Index Items, and Business information component.

[Details][phase-four]

### Phase 5: Extra Time (0.5+ day)

This phase is meant to style our application up, refactor, and add the bonus features.

### Bonus Features (TBD)
- [ ] Make search better so it actually queries the database and valid cities.
- [ ] Make desired landing page.
- [ ] Users can add workspace locations
- [ ] Users can recommend must-trys (favorite food, drink) at a particular workspace
- [ ] Seed data with Yelp API

[phase-one]: ./docs/phases/phase1.md
[phase-two]: ./docs/phases/phase2.md
[phase-three]: ./docs/phases/phase3.md
[phase-four]: ./docs/phases/phase4.md
