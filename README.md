If you want to run the models without downloading NetLogo, you can upload my files to the NetLogo browser version and run them there. I tested it, and it works. Here is the site: https://www.netlogoweb.org/


This is a very simple, abstract NetLogo model on information diffusion. A number of changes were made to an initial model, the SmallWorldDiffusion model, from Ch. 9 of Paul Smaldino’s book Modeling Social Behavior: Mathematical and Agent-Based Models of Social Dynamics and Cultural Evolution. 
The objective was to experiment in simple ways with the dynamics of information diffusion within the NetLogo modeling system. 
Agent-based modeling is a growing field within the social sciences, allowing the exploration of social dynamics that are not easily subjected to experimentation. 
However, it takes practice to master the skills for agent-based modeling and considerable time to develop realistic, plausible models. The work presented here on this small model was not an attempt to develop an elaborate, realistic model, but was rather an attempt to practice the skills appropriate to introductory-level model construction.


The SmallWorldDiffusion model is from the chapter on Networks and constitutes the final model presented by Smaldino in his book. Because social diffusion of information always occurs across networks, this was the appropriate model from which to begin practicing related tools and concepts. 
The initial model consists of identical nodes (individuals), which all have the same degree of connectivity through undirected edges or links. 
It is really a contagion diffusion model, but information diffusion can be treated similarly. A single random pair of individuals is infected, and with guaranteed transmissibility, the infection is spread throughout the network. 
It is a small world network, which means that the network of nodes is clustered, but that some nodes are connected to multiple clusters, enabling jumps of infection across clusters, effectively speeding and widening the scope of transmission. Both clustering and occasional connections between clusters are characteristics of typical social networks. 


Incrementally, I varied attributes of the model. Only the procedure that builds Smaldino’s version of a small world network, a double ring lattice, remains in its original form from the starting model. New procedures have been written, some procedures have been eliminated, and the procedures that have retained their name have been recoded. 
The model now consists of two distinctive types of nodes: disseminators and recipients. The disseminators share their chunks of (abstract) information or arguments with a subset of recipients through directed edges. 
The recipients who initially receive that information can share it with other recipients through undirected edges (any recipient can receive the information first to share with others). The recipients have varying levels of susceptibility to accepting the information or being persuaded by the argument. 
Both the disseminators, who initiate the spread of ideas, and the recipients have varying levels of persuasiveness or effectiveness in conveying the ideas to others. Nodes or individuals who do not accept the ideas steadily build resistance to later acceptance of the ideas. 
They may accept the ideas after initially rejecting them, but after repeated exposure and rejections, they are unlikely to be persuadable. In the final version, both recipients and disseminators have varying degrees of connectivity. All disseminators have random jumps to their connected recipients. However, the recipients retain the small-world network structure. 
That is, the recipient network is clustered, but jumps across clusters are possible. 
The flow of ideas, information, or arguments is tracked by color-coding the disseminators and the recipients. Each disseminator receives its own color. The recipients who initially receive the information from the disseminators obtain a lighter shade of the disseminator’s color. 
Thereafter, every recipient receives the same shaded color as the recipient from whom they received the information or argument. This makes it possible to observe the clustering and degree of spread for the ideas originating from any particular disseminator. If the model is run slowly, it is possible to see the chain of influence unfold. 
The details of the incremental modifications are described for the specific versions. 


To run the model, click on the ‘setup’ button, then click on the ‘go’ button. You can change the speed at which the model runs by moving the ‘Model Speed’ slider in the middle top of the interface. You can pause the model at any time by clicking on the ‘go’ button again. 
If you click ‘setup’ while it is paused, it will reset the model for a new run, so you can choose to rerun the model at any time by clicking on ‘go’ as it is already running to pause it and clicking on ‘setup’ to reset it, and then clicking on ‘go’ again to begin running the newly reset model. 
There are two sliders that you can alter between runs of the model. 
One, ‘num-nodes’ determines how many nodes will be included in the model. It is possible to run up to 1,000 nodes. There will be one disseminator for every 100 nodes. The second slider determines the frequency of rewiring or breaking links to establish new links within the small-world network construction.
If changed substantially, it will affect the amount of clustering and connectedness across clusters. 
I don’t recommend changing it by large amounts from the default because one of the primary points of interest for the model is the degree of clustering that occurs in small-world networks. 


There are a number of interesting models within the NetLogo model library, which may be tangentially relevant to the ways in which I would like to think about information diffusion, epistemic bubbles, and echo chambers. I have only done a simple diffusion model so far. 
The topics that interest me are too complex to do in less than several months' time of dedicated effort. However, I would like to examine the models within the library to glean ideas that could inspire innovative approaches. For example, there are some models that grow networks, such as Preferential Attachment Simple and Team Assembly. 
I would like to work on alternate structures that grow networks. Furthermore, I would like to dynamically break links and forge new links between both recipients and disseminators. Also, this is a very small-scale model, which makes it easier to observe the dynamics, but I would like to develop models with massively larger numbers of nodes or individuals with dramatically more variation in the number of links for them.
