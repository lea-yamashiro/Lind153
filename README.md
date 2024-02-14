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
     $min_x(price)x$ such that matrix $[A, -A] x \geq [b, -b]$
   - Berkeley story: kid gets to class and thinks professor is writing homework on the board, turns out he's solving unsolved problems which arise from Stigler 
   - Times have since changed; the variety of different kinds of food, food prices, and RDI requirements are all quite different from what they were for our grandparents. Why?
      - Nutritional content of foods have changed
      - Inflation (cost of food) and RELATIVE prices have changed
      - SIZES of goods (GMOs)
      - Units – hectograms of food
      - the actual VARIETY of foods available on a given day to a given person is different
      - actual dietary restrictions: based on religion, medical, access
3. Dietary Guidelines for Americans:
   - there is a group of people who, every 5 years, update a list of guidelines for the dietary requirements
      - it'll give a recommended amount of calories, and broken down between different dietary subgroups
      - to make this easier, Ligon made a spreadsheet with all of these values: https://docs.google.com/spreadsheets/d/1y95IsQ4HKspPW3HHDtH7QMtlDA66IUsCHJLutVL-MMc/edit#gid=0
      - we can imagine imposing additional restrictions on a diet based on these numbers and limits (to "lose weight")
    
4. Basic intuition: Linear Program

Think in vector or matrix terms: 
- suppose $n$ different kinds of food
- represent quantities consumed of these as a vector $x$ with $n$ elements
- each kind of food has price; call this vector of prices $p$

Taking the inner product of the price and quantities vectors: 
- a consumer's diet costs $p'x$

Then we have constraints. Each unit of a given kind of food is assumed to provide a set of nutrients 
- suppose $m$ nutrients, then let $A$ be a matrix with $m$ rows, and $n$ columns describing the nutritional content of a single unit of each kind of food
- Different sources of "recommendations" regarding nutrition
   - Equalities: 
