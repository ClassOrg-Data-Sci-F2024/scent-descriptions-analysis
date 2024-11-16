# Progress report 1 
## October 7, 2024
I created the "scent descriptions analysis" repo, and added the relevant files. I found some papers that might be helpful in addition to the Winter (2016) I mentioned in the project idea, and the Jurafsky that was suggested, I also found Hörberg et al (2022) and Poulton (2020). 

I read up a bit on XML which should give me some kind of conceptual grounding for when I actually my data. I also am trying to get a better understanding of emotional valence and valence norms, but I admit, the Winter (2016) was challenging for me.

## Updated: October 28th, 2024
I tried to scrape the "fragrances" page on the wikiparfum site based on the information from the previous class but wasn't getting anything usable, which I am confident is an issue with me and not the page. However, it does seem that the selector gadget tool is having some trouble with this site, so I might need to figure that out. I tried to save the html page as a csv but I think something went awry.

For now, I will just lay out the kind of dataframe I am trying to get to.

Eventually, I'll need to get columns that select for:
- fragrance name
- olfactive classification
- Clasif. Fragrances of the world
- Perfumer
- Price
- Ingredients
- Description
- Concepts

I think at least to start I will replicate the Hörberg et al (2022) olfactory categories to divide the fragrances into the bins "source-based", "abstract", and "evaluative" based on the words in the wikiparfum olfactive classification. I might want to divide further but I'm not certain yet.

I think I will also create subclassifications based on "concepts" and "description", though both might have to get a little creative and I will have to divide based on the presence or absence of certain words decided in advance.

I can then begin to look for patterns in the bin categories vs. the description, price, conecpts, etc. I still think it will ultimately come down to some analysis of word frequencies which will probably then have to be categorized, and then category frequencies. I think I also need to spend some more time with the Hörberg et al (2022) and Poulton (2020) papers, though some of their methods are a little lost on me.

## Updated 16 November, 2024
Thinking through next steps and issues:

I have identified three problems I need to solve to get the dataframe I need:
1. Figure out the css selector issue for a couple of the remaining elements I am trying to capture in their own columns
2. Turn the output from a character count into a string
3. expand the tibble from one link to a random (?) 300

There is still going to be some tidying that needs to happen afterwards but these are the main things.

Next:
I think need to create a separate tibble that lists scent descriptors by category (Using the table from Horberg et al (2022)). I then need to isolate a single column from my wikiparfum df and create a function that will tally the frequency of each category that shows up in the column. So it may be that 3 categories are tallied 3 times each as represented by 15 different words. 

I can then examine any correlation between category frequency and price, represented by three categories: level 1, level2, and level3. So for example I might find that *abstract* is more frrequent in level 3 than level1. 