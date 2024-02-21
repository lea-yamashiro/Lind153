## Planning, February 20: 

Things we need to do before we can do any analysis: 
- Build the diet (pick what foods to compare prices for)
  - How do we want to actually do this?
    - Look at most frequently purchased
      - Find the union of frequently purchased in both regions
      - when you solve those problems, there's going to be some constraint
      - there's microdata from the consumer expenditure survey (CES or CEX) which has detailed data on food expenditures for US households

- Actually record the prices for these foods in each area we're looking at (Safeway prices)
  - Make the spreadsheet things
  - for SF: take minimum cost Safeway, max cost Safeway. Then take Medians 

Then: 
- Create the initial [A] deliverable function that returns the diet (from the notebook "diet_problem.ipynb")
- Then use the linear program to get more accurate and broader inference using the notebook "diet_problem2.ipynb"
