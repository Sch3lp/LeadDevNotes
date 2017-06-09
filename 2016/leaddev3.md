# Mike Gehard - Monolith to microservice
_Pivotal_ @mikegehard

(Make mistakes, safely, in monolith, then migrate that to microservices.)

I don't trust myself to get the bounded contexts right to move straight to microservices.
So I want to get immersive design.

Lookup: realestate-com-au/pact (is this raml?)

**Also look up what those classes are called that represented use cases.**

## Step 1 : api level tests
## Step 2 : Arranging/Organizing your application so you can see your domain
_Lookup: Uncle Bob - Architecture the lost years_
Less costly to evolve bounded contexts and experiment with boundaries
Delaying architecture decisions
## Step 3 : Break out components
Give more space in the codebase and solidify dependencies/boundaries.
Like having a brick walls between boco's.
Migrations only touch one table.
## Step 4 : Promote your microservices
e.g. if you want to scale a certain boco,  or multiple app's want to talk to that boco.
Introduces additionial costs: Network communication issues
You'll have to introduce Service Discovery.
You'll have to introduce a Circuit Breaker (to deal with network partitioning).
## Step 5 : Continue promoting microservicees
Because we've built necessary stuff around it.
