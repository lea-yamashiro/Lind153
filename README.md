### Idea of this project: 
What is a subsistence cost diet?

What kinds of populations might this be relevant for?
 - country going through famine
 - country going through some natural disaster
    - need to fly in relief
    - money, time, how to cover a starving population... 
 - isolated areas, like rural areas
 - refugees, refugee camps 
 - prisons: making sure prisoners are adequately nourished but minimize cost 
 - food deserts?
 - Schools?
 - Military
   - Studies have been done on feeding the military
   - involves explicitly trying to calculate minimum cost diets for soldiers in the field
   - took volunteers and gave them extremely minimal diets, as a way of finding out how to keep the military adequately nourished during wartime
  
We'll think about different types of diets in this project. The main problem: 
- the lowest cost possible diet, and the list of nutrients.

Walking through steps of the project: 
1. Introduction: the idea is to solve the problem of finding the minimum cost diet satisfying a set of "Recommended Dietary Intakes" (RDIs) for a particular set of parameters.
2. History: problem was first "solved" by Stigler (1945) for a set of foods and prices and RDI requirements (Dantzig 1990) for an entertaining discussion of what "solved" meant in that context
   - he created a "linear program"
   - where you have some vector, that looks like
     $ min_x (price)x$
     such that
     matrix $[A, -A] x \geq [b, -b]$
   - Berkeley story: 
    - Times have since changed; the variety of different kinds

