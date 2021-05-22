## maven-package-problem

# What I want to do:
I have a Server and a Client Application that share some common Code (some Datastructures).
And to avoid Code duplication I want to share this common code between my Client and my Server.

# The way I approched this Problem:
I tried to solve this by macking a multi-module Project.
I extracted the common code into a module and created a module for the Server and the Client.
then I added the Shared code as a Dependency to the Server and the Client and added both depndencys in the dependency manager of the aggregator pom.

# The Problem I encountered:
now since this is just a small part of the whole Project(hence this simplification) I wanted to structure the modules internaly with java packages.
But I can't use the shared code inside java packages (as demonstarted by the ClientDataManager1) but I can use it outside of this java package (ClientDataManager2)

# My Questions:
1. Is this even the right approach for this Problem or should this be solved in another way ? And if so how ? And where could i find more resources on that approach?

2. If this is the right approach how can i structure the Modules internaly (or use the shared code inside of java packages)

Thank you for taking the time to answer my rookie questions.
