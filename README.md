# Badger NFT’s

Description is available at https://docs.google.com/document/d/1aXSyTcQLwGvnhJ7oVsv1oo8RI2k9mj6t2wJ9mYPnXeY/edit

## Baseline 

As a baseline creation mechanism for NFTs we consider https://github.com/HashLips/generative-art-opensource/tree/main that generates the X number of pictures based on the configuration that you set. Particularly, the repository allows for multiple layes and specified rarities for for certain rarity/layer combinations. In fact, `addRarityPercentForLayer` allows for more fine grained control over how much randomness there should be during the generation process, and allows a combination of common and rare parts.

[Youtube Tutorial](https://youtu.be/NIJI2_1anqA)

## Rarity Specification Challenge

> The challenge also becomes how to define the rarity allocation. Should certain attributes carry more weight? Should x # of attributes on a badger define rareness, or should it be defined on the rarity of each separate attribute. Maximum attributes per badger would be 8 (hat, hair, chain, smile, beard, cig, glasses, earring) but for aesthetic purposes 5 seems to be the fitting max.

We propose for a each picture to have a maximum amount of attributes as 5 out of 8 available attributes. Besides, we propose to define rarity in terms of each attribute, which will promote diversity and identify the most rare ones as consisting of the combination of the rarest features.

> There is also the issue of series, currently we have a wrestling series which includes ~10 designs which are a combination of attributes. We also have a number of badgers made by hand for our community. It would be nice to have a way to fit these into the scheme. Submission of rarity models can help us break down the allocations and set the baseline for us to develop the generation of the badgers. One concern becomes the # of colours on the palette used to generate the base layers & attributes. How can the colour scheme define rarity? Should background colour perhaps define rarity?  Not all badgers should have all traits, and it would be best if they combined in a way that was generally aesthetically pleasing and/or interesting.

To reward a custom-made avatar, - creator's attribution sounds as a great idea in the description of the NFT.

The backround colour could define/map to a particular location. For example, green being a football field and yellow being a seaside. Another possibility is that a colour could map to a feeling such as red - anger, blue - sadness.

In my opinion, GPT-3 generated description can further enhance an avatar, create unique experience and make the project more exciting.

Some ideas on GPT-3 interactions:
- [The first intelligent nonfungible token|GPT-3 Demo](https://gpt3demo.com/apps/to-the-young-artists-of-cyberspace-inft)
- [A robot wrote this entire article. Are you scared yet, human?|Guardian](https://www.theguardian.com/commentisfree/2020/sep/08/robot-wrote-this-article-gpt-3)

## Distribution of Attributes

For the fare distribution of atttributes we advocate first expicitly defining a maximum of 5 attributes with an option of having less than 5 attributes for each avatar. 

Process for distributing attributes:
1. Define probability for each attribute, for instance, as 2.5%, 5%, 7.5%, 10%, 15%, 30%, 50%, 70%. After an attribute is used we make the probability equal to 0.
2. Within each attribute assign probability to each item in a similar fashion. Include a possibility of no item, thus effectively not utilizing an attribute.

### Advanced Distribution

For more details on the distribution of attributes we suggest using [binomial distribution](https://en.wikipedia.org/wiki/Binomial_distribution) which we encounter in [Crypto Punks](https://www.larvalabs.com/cryptopunks/attributes).

![image](https://user-images.githubusercontent.com/66903336/132584846-d280ba44-1075-4c93-aa68-129b4d5cd604.png)

![image](https://user-images.githubusercontent.com/66903336/132585038-23d28ed6-4df1-409d-94bc-56ce32801327.png)

