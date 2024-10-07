## Summary
English has no smell descriptors that aren't methaphoric, which opens smell descriptions up to a lot of creativity. But metaphors by their nature are inexact, if poetic. I think this gives rise to a range of interesting questions, such as those which center on semantic maps and sociolinguistic ideologies around sense (that is, the chemical kind, not the "and sensibility" kind), particularly those which involve a sense (an altogether new definition of the word) of value or even class. Using data scraped from the website Wiki Parfum, I will search for patterns between the descriptions of their database of perfumes as they relate to each other and to their price categories, and try to draw conclusions about societal assumptions about certain olfactory words and their associated values. 

## Questions
1. Do we find certain semantic categories are associated with greater or lesser monetary value?
2. Do these categories contain words with similar valence scores (can use Mohammad (2012) and Warriner (2013) as a reference), and how might this help predict associated value?

## Data and Analysis
This project will use data from https://www.wikiparfum.com/en/, which is a large database of perfumes, their descriptions, their prices, and ingredients.

When asking the site's chatbot where the perfume descriptions come from, I get the following answer:
"The descriptions of perfumes are created by experts in the field, often including perfumers and fragrance houses. These descriptions aim to capture the essence and experience of the fragrance." I don't know that its possible to get a better answer, but I think its likely the descriptions were pulled from the original (English) websites. I can also infer that they are geared towards a largely Western audience.

I need to figure out a way to scrape the data, but it seems to be in a relatively usable form. If I choose to pursue the semantic categories question (and I think this will remain somewhat open until I look through the data more closely), I will need to develop some method of creating them. I think using existing emotional valence categories might be one way to go about this. Alternately, Hörberg et al (2022) organized a group of 243 olfacotry words along the guidelines of Poulton (2020), into the categories "source-based", "abstract", and "evaluative". It could make sense to duplicate these categories, or use them as a guide. 

The way these categories are created will change how the data is analyzed, but I think I have to analyze word frequenecies in some way as a function of price category. 