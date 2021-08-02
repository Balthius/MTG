
# Create a Tableau Story


## Table of Contents

* [Links](#Links)
* [Summary](#Summary)
* [Design](#Design)  
* [Feedback](#Feedback)
* [Resources](#Resources)


## Links


## Summary

In this visualization, I compare how Wizards of the coast have chosen to balance their content over the years
Some prior knowledge to help understand the dataset:
- **cardName**: The card name, A Unique Identifier
- **superType**: A 'Special' identifier on the card, which dictates certain *specific* rules that must be applied to them in addition to the normal rules
- **cardType**: The types of a card (i.e. Creature); applies a more general set of rules to the card, every card will feature a type, or combination of types
- **subType**: The subtype of a card (i.e. Human)indicates certain behaviors this card will adhere too, as well as allowing for readily identifiable synergy between other cards sharing a subtype
- **convertedMana**: The converted mana cost of a card; This value roughly indicates how powerful the card is, especially when paired with rarity.
- **cardSet**: The set this card was printed in.
- **rarity**: The rarity of a card; string
- **releaseyear**: 1:1 with the card set, but far more useful for data analytics

As more sets are released, and Wizards of the Coast gets more feedback on how players are interacting with their content, we can see their content begin to stabilize (as seen with Rarity and subtype), and we are also able to see a few examples of Wizards of the Coast using community interest to generate new content that appeals to a variety of audiences (Commander, Modern, as well as others not pointed outin this exploration).

Another great example of player feedback being recognized is the explosive number of 'legendary' supertype cards printed. this is a limiting supertype, but with the release of things like Commander that explicitly depend on building around a selected 'legendary' card, WotC is showing responsiveness to their community's preferred formats rather than exclusively pushing their 'standard' format.

Data from https://github.com/yhejazi/mtg-web-scraper thanks to Yasmine Hejazi

[Updated Version of the Story](https://public.tableau.com/app/profile/josh.folsom/viz/Version4MTGTableauExploration/MTGStory?publish=yes)
## Design

### Version 1
- [Card Type and Subtype: Rarity Dashboard](https://public.tableau.com/app/profile/josh.folsom/viz/CardTypeandSubtypeRarityDashboard/CardTypeAndSubtypeRarityDashboard?publish=yes)

Which gives some numerical overviews on cards, with a filter for rarity, and a filter for subtype, both to reduce visual clutter as desired.

- [Rarity and Subtype Dashboard](https://public.tableau.com/app/profile/josh.folsom/viz/RarityandSubtypeDashboard/RarityandSubtypeYearDashboard?publish=yes)

This Dashboard is Centered on Year as the tweakable value, with Rarity as a second, lesser knob

- [Year and Rarity Dashboard](https://public.tableau.com/app/profile/josh.folsom/viz/YearandRarityDashboard/RarityYearDashboard?publish=yes)

The third displays the trend, by year, of release-by-rarity

While tweaking values, I wanted users to notice that humans are a very prolific subtype. This seems to be less about favoritism, rather, it seems to be a lore-driven decision; This is almost more about the extraordinarily invasive nature of humans, finding their way into every nook and cranny available.

From a outside-the-game metaperspective, it seems that over time we've seen a increase in all well-represented rarities, but the rate of increase is very proportional to the total count of cards for that year. Common will always be the most prolific, but we can see that in years with many Mythic rares, we'll also see a large surge in commons. Therefore it seems that there is some sort of ratio that Wizards of the coast likes to adhere to, one which theyve in fact improved voer time. It's only in the earlier years that we see some rare/uncommon values being 'out of place'

### Version 2
I decided to remove 2021 Data since it is incomplete, and affecting some important visualizations (313 Data Points, less than 1%)
restructured my sheets to work better with stories

Tried to handle many of the questions by adding some prior knowledge. 

- [Version 2](https://public.tableau.com/views/Version2MTGTableauExploration/MTGStory?:language=en-US&publish=yes&:display_count=n&:origin=viz_share_link)

### Version 3
Clarified some language for better readability and explanation, split up the last dashboard. 

- [Version 3](https://public.tableau.com/app/profile/josh.folsom/viz/Version3MTGTableauExploration/MTGStory?publish=yes)
## Feedback

### Version 1 
 
* Common will always be the most prolific. . . but it seems that there is some sort of ratio that Wizards of the coast likes to adhere to, one which theyve in fact improved voer time. It's only in the earlier years that we see some rare/uncommon values being 'out of place'
    Question: What does that paragraph mean?

* I noticed sub-categories of Creature were in same alpha list. i.e., Alpha Creature, Enchantment Creature, Instant Creature, Land Creature. . . so does the total of these categories = 17,613?)
              
* Human appears in several separate categories (i.e., Human Wizard, Human Soldier, Human Cleric, Human Knight, Human Warrior) but I don't see a total for all the sub-types in the second table like I saw for 'Creatures' in the 1st Made me curious. . . why? I don't know anything about the game - card types or subsets - so can't infere why the general category "Creature" would appear together with it's subsets in the first table, but the same principle would not be used for a general category "Human" (together with subset humans) in the second table.

*Why are all the bars the same color in the 2nd bar graph? (Common, Rare, Uncommon all navy)

* I would need to see all three Dashboards together to be able to remember what cards are Common, Rare, etc. so I could interpret what cards the colored dots stand for. Without that, I don't have the necessary labels that inform me what the increases since 2008 mean. I see definite increases and definite trends, but can't know whether those are Creature, Human, Sorcery, or______ cards.

* Is is possible to create a colored bar graph showing the general categories of Human and Non-Human cards?

* Possible to create a colored bar graph that compares the general categories of Creature, Human, Sorcerer, and all other pertinent general categories? If so, perhaps I could get a quick visual comparison that would allow me to see immediately the ratio of "human" cards in comparison to "non-human" cards.

* I'm highly informed by a) colored bar graphs and b) comparison tables to show me relationships.

* Stand alone numbers give me general information like the prolific appearances of Creature, Enchantment, Sorcery, and Land. This suggests to me that land is where sorcery happens and much of it has to do with creatures and enchantment. 

* That said, I do see by the Grand Total column in the Subtype by Rarity, that humans play a significant role in this game. Not knowing the game, I don't know if they pair up with sorcerers and creatures or not. Don't know what their relationships are.

* A colored bar graph that shows the totals of general categories together with the sub-sets that make up the colored categories would also help me see at a glance relationships and/or trends.

* Colored bar graphs are immensely helpful for non-gamers like me.

* Need to see all the stuff together. I found the "by Year" table informative in noticing there was a steady increase, but I didn't know what it represented because I had to look at it apart from the other tables.

* Why Dashboards had to be separated. I know it had to do with technical parameters, but it shaped my ability to interpret the graphic all the way through.
  
* Can't infere why "Creature" would appear together with it's subsets in the first table, but the same principle would not be used for a general category "Human" (together with subset humans).

### Version 2
Specific things I liked about it:

a) Where it was positioned right up at the top
b) Easy-to-use arrow format that let me scroll back and forth at will
c) Easy-to-follow explanations!! (Especially helpful for a non-gamer.)
d) Slender horizontal field that didn't interfere with seeing the tables/graphs below
    *Kept the helpful guidance in same visual field as data. VERY NICE!

The 3 List: Set Release Count by Year
   a) Really helpful visual aid!
   b) Concise, see-at-a-glance the sets over a span of almost 30 years
  
Comment: Intrigued by the sharp "peaks" during certain years. What factors contributed to sharp peaks in '98/'99 and '2013/14? How would this inform me as a game manufacturer? Coder? Marketer? Seller? Gamer? Stock broker? Social historian?

Bar Graph: Rarity Count by Year
   a) Concise, see-at-a-glance graph.
   b) Intrigued by the close correlation between all the types (Common/Uncommon/Rare) except for Mythic Rare, which seems not to even show up until 2008 and is proportionately below the others from then on. Not sure what that means for gamers and how they experience the game.

Histogram
   a) A great visual aid!
   b) Immediately noticeable surges, like that of the Spirit card. In 2002, None. . . . in 2004  57  . . . in 2005  104 !?

*I noticed this in the Year Released Sub type table, but it shows up most dramatically here. Why would there be such a dramatic change in the span of 5 years among game producers/gamers? Is this related to world events? Popular movies? Music? Best-selling books released? New technology inventions and/or aps? Other?
     
LineGraph: Supertypes by Year
Definitely needed your explanation to orient me to how to interpret this one.

First, I looked at the color key to the left a couple of times to remind me what the lines and dots meant. THEN, I realized my cursor on each colored line would give me the name of the card, the year of its release,  and count. NICE!! Very helpful little text box.

My mind didn't interpret the results as "more balance." Here's what my mind did:

I looked at the green line so far above the other colored lines and thought, "Hm. Why is there a growing imbalance in Legendary?"

Similarly, when I saw the purple line dropping and drooping, I thought, "Why did Snow drop off so suddenly after its initial release?. . . and  Why does it disappear until 2013 and creep along at the bottom from then on?"

These raise the question of how does one correctly interpret the results if one is a non-gamer? The only way would be by having the helpful hold-your-hand-and-guide-you-to-the-right-interpretation paragraph above the chart. :)

## Resources

- http://gamapserver.who.int/gho/interactive_charts/mbd/life_expectancy/atlas.html