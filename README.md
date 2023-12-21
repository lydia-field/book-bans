# Partisan Discussion Around Book Bans in the United States

Social Media Analysis Group Final Project
Lydia Field, Joshua Weinert, Elias Schimkat, Haley Vandall

## Abstract

Over the past year (2022-2023), book bans in public schools and libraries have been a hot political topic in the United States. Republican-led states like Florida and Texas have banned books that allegedly contain references to sex, “Critical Race Theory”, pornography, and LGBTQ+ issues. Florida governor Ron DeSantis has been an outspoken supporter of the bans, claiming that children should be protected and that reading material in schools should be “age-appropriate”. Democrats and political leaders in Democratic states like California and New York have spoken out in opposition to book bans, asserting that the material in question is not only age-appropriate and has been in school curricula for decades, but that it’s also entirely innocuous. Twitter, the social media platform known for being rife with political discussion, has served as a host for this conversation. In analyzing partisan discussion around book bans on Twitter, we found that there are some key topical and lexical differences between the ways in which individuals in pro-book-ban states and those in anti-book-ban states engage in conversation. However, we also found that, in lexicon alone, there is a significant degree of convergence between the two sides. Looking at this phenomenon in conjunction with the overall context of the conversation and of presumed partisan positions, we conclude that engagers in pro-book-ban states discuss justifications for book bans while engagers in anti-book-ban states use similar vocabulary to express their opposition to the bans. This result implies that there is a direct partisan opposition in this topic, with little middle ground.


## Research Question: 

**How does partisanship impact the most common justifications for book banning (Religion, Race, Pornography) in the United States? Are there significant topical and lexical differences between discussions around Blue (Democratic) and Red (Republican) states?**


## Background information

Book banning has been a topic of political discussion in the United States for decades. Books like 'To Kill A Mockingbird' and 'Of Mice and Men' have oftentimes been considered controversial in the US–whether due to explicit language or mature topics–and removed from classrooms (Harvard 2023). Book burning was a key tactic of censorship by the Nazis in World War II, with the aim of controlling and limiting access to information. Today, book bans are highly controversial, and easy access to information via the internet makes it so that what can be found in a book can be found elsewhere. Nonetheless, they have become a core example of partisan controversy in recent years, as American political party platforms have become more staunch.

Book bans are most often enacted by Republican state leaders, most notably Florida governor Ron DeSantis and Texas governor Greg Abbott, and have become a common campaign point for other members of the Republican Party. They have also become a frequent subject at school board meetings across the country, where parents (generally conservative or Republican-aligned) voice their concerns about available reading material in public schools and libraries. Typically, their concerns stem from worries over “age-appropriate” subjects and “personal” topics. Common “controversial” topics include explanations of sex, depictions of LGBTQ relationships, and discussions of racism and “Critical Race Theory” (Meehan & Friedman 2023). Although book banning is an independent issue, much of the discussion parallels other partisan debates.

In the past five years, over 300 books have been banned in educational institutions in Florida alone, marking the highest rate of book banning yet (Gilbert 2023) and PEN America reports that 1,477 books have been banned across the country in 2023 (Meehan & Friedman 2023). This increase in bans has led to pushback from many citizens and political leaders, primarily members of the Democratic party. Opponents of book bans broadly disagree with censorship of speech and feel that book bans may increase instances of discrimination, threaten freedom of speech, and risk LGBTQ+ rights. They also criticize the fact that, often, the content deemed “controversial” or “harmful” by book ban supporters, is being misconstrued, misinterpreted, and falsely demonized. Morality is often invoked by engagers on both sides of the discussion, with book ban supporters arguing that bans allow parents to decide what their children should be learning and opponents emphasizing the potential detriment to child development and learning.

The discussion of book bans, both within legislatures and on public fora, is ongoing and evolving. California and Illinois have enacted legislation which effectively bans book bans in the states, and several other Democratic-led states are set to follow suit. President Biden has promised to appoint a “book ban point person” in an attempt to combat and track the bans on the federal level, but Republicans remain steadfast in their position, which is likely to be emphasized during the run-up to the 2024 election (Ukenye 2023).


## Our Process

In order to examine public opinion around book banning, we decided to use Twitter conversation as the basis for analysis. Although Twitter, and social media in general, provides a limited context and cannot necessarily be extrapolated to reflect reality, it is still a good measure of public opinion. The structure of Twitter encourages users to be opinionated, and engagement on posts is a good measure of public interest in discussions. Additionally, Twitter is often used by politicians, political commentators, and politically-engaged citizens to discuss important topics in real time. Given that the subject of book banning is very controversial and opinions on it generally follow partisan ideological lines in the United States, it is likely to be a hot topic on Twitter. 

The partisan nature of the conversation, too, provides an interesting point of analysis for our research. In the United States, Republicans and conservatives are generally more likely to support book bans, while Democrats and liberals tend to favor open access to information. Therefore, we formulated our research question around this partisanship. It is often difficult to make assumptions about individual Twitter users’ political leanings, so we used US states as a proxy variable to analyze partisan opinions. Policies around book bans in the US also vary considerably depending on the state and state leadership, so comparing state discussions is likely to illuminate differences in opinions. 

In order to make some generalizations about partisan leaning and its correlation with opinions on book bans, we compared “red” states (Republican or pro-book ban states) and “blue” states (Democratic or anti-book ban states). We also did a deeper case study analysis between one state from each party: Florida and California. We chose these states to represent their parties because each state has recently passed legislation regarding book bans, and both state’s governors have been active on Twitter regarding book banning. 

**Therefore, in this project we aim to analyze the key lexical differences between red states and blue states’ discussion of book banning.**


## Methodology

Using meltwater, a proprietary tool which scrapes from the Twitter API, we compiled a dataset of 20,000 tweets using the query: (book OR books) NEAR (ban OR bans OR banning OR banned OR bannings). The publication date of the tweets spans November 25, 2022 to November 28, 2023. The full dataset of tweets from this query and time period includes over 1.3 million posts. We removed retweets and took the top 20,000 posts by engagement, which results in a representative sample of influence and discussion on this topic. We also conducted some preliminary data cleaning to remove null values, empty columns, and most hyperlinks. 

We then segmented the data for more thorough analysis according to our research question. We looked at the breakdown of tweet origin by US state and mentions of US states to determine the top 5 Republican/conservative states and the top 5 Democratic/liberal states. Based on these statistics and general news about book banning in the United States, we chose to analyze the following states: 

* **Democratic (blue states):** California, New York, Illinois, Massachusetts, Washington
* **Republican (red states):** Florida, Texas, Utah, Missouri, Pennsylvania*
  * (Pennsylvania is a Democratic state, but has the third-highest number of banned books, so for our purposes it is considered a red state.)

We then compiled tweets for each state using mentions of state names and abbreviations, state keywords, governors & other political leaders, counties, cities, geographic origin, and tweets authored by governors & other political leaders. Because tweets often mention more than one state at a time and governors of one state tend to discuss affairs in other states, there is some overlap in the lists of tweets. In analyzing each state individually, we did not dedupe the lists, as all mentions of that state are relevant to the analysis. However, when we compiled the subsets into groups for blue and red states, we removed duplicate tweets so as not to skew the results.

To analyze this data, we wanted to focus on keywords and topics, to determine if there is a tangible difference in the way red and blue states view and discuss book bans. Therefore, we created BERT topic models, LDA models, and lexical analysis models for the entire dataset, the blue state group, the red state group, and Florida and California individually (for a more specific case study).

We did encounter some methodological limitations during this process, but none which are likely to skew our analysis. First, “quote tweets”, posts which comment on a tweet from another user, contain both the commented tweet and the original tweet in the dataset. This means that even when deduping the data, there is some duplication. This may make certain keywords seem more common than they actually are, as many users may respond to one tweet (therefore making that tweet appear several times). Second, we found it difficult to remove all stop words and common non-specific verbs (like “like”, “want”, and “do”) from the data. This may suppress other, more telling keywords by ranking them lower (on lists of most common words). Despite these limitations, we were able to create a robust picture of the common lexicon and debates around book banning in the United States. Third, our method for deduping the red and blue state groups involved combining the two datasets, shuffling it, and then removing duplicates. Because the deduping process removes the first duplicate (and each tweet may fall into both the blue and red categories), the shuffling makes it so that different tweets may end up in the blue and red categories each time. However, the difference is negligible and does not impact the results.


## Analysis

### Descriptive Statistics

| Grouping | State | Post Count | Engagement |
| --------- | ------ | ------ | ------ |
| Blue  | California | 1,913 | 3,816,166 |
| Blue  | New York  | 2,026 | 2,606,770 |
| Blue  | Illinois | 1,205 | 1,564,113 |
| Blue  | Massachusetts  | 384 | 464,314 |
| Blue  | Washington  | 1,120 | 1,256,302 |
| Red  | Florida | 5,501 | 6,148,246 |
| Red  | Texas | 1,641 | 1,343,758 |
| Red  | Utah | 397 | 280,354 |
| Red  | Missouri | 514 | 473,462 |
| Red  | Pennsylvania | 790 | 665,259 |

**Blue States:** Among the “blue” states, New York had the highest tweet volume, but California tweets saw notably higher engagement. This implies that while New Yorkers (with a high concentration of media companies) frequently discuss book bans, the topic itself is not as popular among the New York audience. This is likely because book bans are unpopular in New York state and discussion more often focuses on bans in other states. In California, Governor Gavin Newsom is an outspoken opponent of book bans, and the state’s liberal majority tends to engage on social media in opposition to right-wing viewpoints. Illinois, which was the first state to pass legislation banning districts from banning books, also drove a notable discussion. Washington and Massachusetts drove some discussion, but neither states have been major players in the book ban conversation overall (they provide additional representation for Democratic states).

**Red States:** Among the “red” states, Florida had by far the highest volume of tweets and engagement. The book ban discussion in Florida tends to make national news, meaning that much of the discussion about Florida comes from engagers from other states. Texas, another Republican stronghold, also saw a high volume of tweets, largely discussing Governor Greg Abbott’s position and comments on book bans. Pennsylvania is a bit of an outlier, as it is a swing state, but has the third-highest number of book bans in the country. Interestingly, Pennsylvania drove a larger and more engaged discussion than the more strongly conservative states of Utah and Missouri. 

| State Group | Post Count | Engagement |
| --------- | ------- | ------ |
| Blue States  | 4,942 | 7,217,916 |
| Red States  | 6,328 | 5,883,267 |

*These combined datasets have been de-duped*

Although red states drove a substantially larger discussion around book bans than blue states, blue states actually drove a higher total level of engagement. This implies that many of the “Florida” tweets (Florida drove the highest engagement for any individual state) are posted by residents and engagers of blue states. This could also imply that posts from blue states are more likely to go viral, while red states are more passive subjects of discussion.


### Case Study Selection: 

We chose to focus on Florida and California as they are the two states of their groups with the highest engagement, indicating a high attention towards book banning in their states. Additionally, Florida has the highest tweet count out of red states and California has the second highest tweet count of blue states, after New York. However, since New York contains a high amount of media outlets, many of these tweets come from agencies over constituents, further justifying our selection of California.


### Temporal Analysis

#### Full Discussion

Conversation as a whole began to tick up in January of 2023, peaking at the end of May. Discussion declined over the course of the summer, likely because public schools, the biggest context for debate over book bans, were not in session. Discussion saw some moderate spikes in September and again in mid November. Engagement followed a similar trend, although at a much lower volume. On January 18, 2023, a tweet from Stephen King condemning bans on books went viral, driving a massive, anomalous spike in engagement. Two of the largest spikes were driven by discussions of book bans in Florida. 

**Full Discussion Posts & Engagement Over Time**

!['Full Discussion Posts Over Time'](https://github.com/lydia-field/book-bans/blob/main/data_images/all_tweets_time.png?raw=true)

The first major spike in post volume occurred on March 24, 2023, when Florida passed the “Parents’ Bill of Rights” legislation, allowing parents more control over their children’s education and restricting the use of “personal pronouns” in public schools (Atterbury 2023). Posting volume peaked on May 24th after Florida schools banned Amanda Gormon’s 2020 inauguration poem (Chappell 2023). After a few months of limited discussion, posts spiked again on September 12, 2023 after Illinois passed legislation banning book bans in public schools and libraries (Savage 2023). In general, discussion volume was heavily dependent on relevant news moments. Book bans are incredibly controversial and polarizing in the United States, thereby drawing a continuous, but ever-changing conversation.


#### State-by-State

As expected, Florida drove the highest posting volume and engagement over the course of the year. Both posts and engagement saw major spikes in February and May 2023. Other spikes also experienced spikes in conversation in May, but not in February. This implies that discussion in February was solely focused on book bans in Florida, while the spike in May included conversations about other states. California saw the second-highest level of engagement consistently over the years, but only saw the second-highest posting volume in two months out of the year. California tweets tend to gain significant attention because its governor, [Gavin Newsom]([url](http://twitter.com/GavinNewsom/statuses/1678106495475433473)), is active on Twitter and is considered a strong leader within the Democratic party. 

**All States Post Counts**

!['All States Posts'](https://github.com/lydia-field/book-bans/blob/main/data_images/all_states_time_count.png?raw-true)

**All States Engagements**

!['All States Engagements'](https://github.com/lydia-field/book-bans/blob/main/data_images/all_states_time_engage.png?raw-true)

New York and Texas dominated discussion volume behind Florida. Discussion in Texas spiked in April 2023 when a public library in Llano considered closing down after a federal judge ordered banned books to return to the shelves (Serrano 2023). Discussion in New York remained elevated between February and May, spiking in May around news that the Brooklyn Public Library would open its entire digital collection to children ages 13-17 in an effort to combat censorship and book bans. Discussion in New York also commonly followed a similar trend to Florida, as engagers from New York often criticized DeSantis’ and others’ positions on book bans. The spike in discussion and engagement in June 2023 around Illinois’ ban on book bans contributed to spikes in national discussion (Savage 2023).

**Florida & CA Posts & Engagements**

!['FL & CA Posts'](https://github.com/lydia-field/book-bans/blob/main/data_images/fl_ca_time.png?raw=true)

In comparing Florida and California directly, we can see that precise spike moments were distinct. California’s discussion did not spike in February and May like Florida’s, but rather spiked in April and July. Florida’s post volume and engagement tended to trend together, experiencing parallel spikes. California, on the other hand, often saw engagement that was disproportionately high compared to posting volume month over month. Most notably, engagement in April 2023 was nearly proportionately double the posting volume. This was driven by a barrage of tweets governor Gavin Newsom received, criticizing him for opposing book bans in Florida. Newsom’s [original tweet]([url](http://twitter.com/GavinNewsom/statuses/1646184293306339328)) received significant engagement as a result, and several of the [responses]([url](http://twitter.com/JeremyRedfernFL/statuses/1646325922033696771)) to it did as well, driving up overall monthly engagement. A similar spike occurred in July, when right-wing commenters responded to Gavin Newsom’s [tweet]([url](http://twitter.com/GavinNewsom/statuses/1675613117789896704)) supporting an anti-book-ban bookstore in Boise, Idaho.


#### Blue & Red States

**Blue & Red States Posts & Engagement**

!['Red & Blue States'](https://github.com/lydia-field/book-bans/blob/main/data_images/red_blue_time.png?raw-true)

When grouped, red states and blue states all saw elevated discussion volume between February and June 2023, with red state conversation peaking in May and Blue state conversation peaking in April. Red states generally saw higher discussion volume than blue states, but that began to shift towards the end of 2023. However, blue states tended to see higher engagement month over month. Blue states’ higher engagement numbers could imply that there is a level of fascination with right-wing viewpoints among a liberal audience. Florida still drives the majority of discussion across both groups.


### Keyword & Topic Analysis

#### Full Discussion

Top keywords appearing in the overall conversation represent the context of the overall discussion. These include: “student”, “library”, “school”, and “children”, revealing that most discussions involve book bans at public libraries and schools and primarily concern the interests of children. “Republican” and “GOP” are often commonly referenced, while “Democrat” is not, implying that a large contingent of the discussion criticizes the Republican party for making book bans a de facto element of its platform.

**Top 20 Keywords - Full Discussion**

!['All top 20'](https://github.com/lydia-field/book-bans/blob/main/data_images/all_top_20.png?raw=true)

For the **full discussion**, the top topics, in order of coherence, are: 
1. **Mass Shootings** (“guns”, “weapons”, “assault”, “shootings)
2. **Age-Appropriate Material** (“appropriate”, “parents”, “age”, “children”)
3. **Illinois** (“Illinois”, “pritzker”, “jb”, “giannoulias”)
4. **Moms for Liberty** (“moms”, “liberty”, “group”, “hate”)
5. **Race** (“black”, “white”, “racism”, “history”)
6. **Pornography** (“porn”, “pornography”, “explicit”, “sex”)
7. **Fascism** (“fascists”, “fascism”, “powerless”, “women”)
8. **Iowa**  (“iowa”, “reynolds”, “iagovernor”, “iowans”)

**Full Discussion Topics**

!['All Topics'](https://github.com/lydia-field/book-bans/blob/main/data_images/alltweets_topics.png?raw=true)

The top topics for the overall conversation around book bans in the US follow common media narratives around the topic. Topics 1, 5, and 7 represent narratives used by liberals and those opposing book bans to push back. Book ban opposers often hit back on those advocating for them, criticizing the narrative of child safety, as many people on the right who support book bans also oppose gun control legislation. Liberals will often respond to conservatives by saying that mass shootings and unregulated guns are more of a threat to school children than books. Race and racism are also discussed by those opposing book bans, as they believe that discussions around race and racism should be part of public education, unlike those who support book bans. Finally, those opposing book bans often invoke the label “fascist” when discussing book ban supporters, accusing them of advocating for excessive government control over education and speech. 

Topics 2, 5, and 6 are common narratives used by conservatives and those advocating for book bans. Book ban supporters often argue that books should be “age appropriate”, meaning they should not discuss “complex” or “controversial” topics with young children. This is a common justification for banning books that contain mentions of sex, LGBTQ+ issues, and race. Race and “critical race theory” are often also used as reasons to ban books, as book ban supporters claim that discussing race and the history of racism in schools could lead to more societal divisions. Book ban opponents, on the other hand, view this position as the erasure of history. Finally, book ban supporters often claim that books contain “pornography”, although very loosely defined. Many books have been banned because they allegedly contain explicit references or discussions of sex, but supporters use the term “porn” as a red herring to force the issue. 

The three other top topics discuss Illinois, a state which has banned book bans, Iowa, another state which has come under fire for banning books in public schools, and “Moms for Liberty”, a right-wing group. “Moms for Liberty” is a common voice in the book banning conversation, often being one of the first to amplify news of the bans. Its members attend school board meetings across the country advocating for banning books that are not “age-appropriate”. The group is discussed by both conservatives, who tend to agree with them, and liberals, who staunchly oppose their activities and often refer to them as a “hate group”.


#### Blue & Red States

##### Blue States Keywords

**Top 20 Keywords - Blue States**

!['Blue Top 20'](https://github.com/lydia-field/book-bans/blob/main/data_images/blue_top_20.png?raw=true)

Top keywords used by **blue state** engagers tend to mirror those used in the overall conversation, but “Florida” and “@GavinNewsom” are uniquely common to blue states. This supports the finding that Florida is a common topic of conversation in general, and liberals from blue states often engage to criticize its politics. California governor Gavin Newsom is commonly referenced because of his staunch opposition to book bans and the strong support he receives from fellow Democrats.


##### Blue States Topic Model

**Blue States Topics**

!['Blue State Topics'](https://github.com/lydia-field/book-bans/blob/main/data_images/blue_states_BERT.png?raw=true) 

In **blue states**, the most common topics, in order of coherence, are:  
1. **Illinois** (“illinois”, “pritzker”, “legislation”)
2. **California** (“california”, “newsom”, “gavin”, “ca”)
3. **Moms for Liberty** (“moms”, “liberty”)
4. **Ron DeSantis** (“Desantis”, “Ron”, “Florida”, “Trump”)
5. **Abortion** (“abortion”, “women”, “pro”, “anti”), LGBTQ+ (“queer”, “lgbtq+”)
6. **Pornography** (“porn”, “pornography”, “explicit”), and race (“black”, “history”, “racism”)

Generally speaking, **blue states** had a high frequency of words often used in connection book banning, such as "nazis", "misinformation", "fascist", "facism", or "fascists" as well as "bullshit". This represents a broader narrative surrounding the topic, in which its opponents claim that book banning can be compared to the above terms, whereas the proponents assert that certain books are filled with “misinformation” about, for example, gender identity. Furthermore, political figures and states introducing book ban laws such as "Florida" and "Texas" as well as their governors such as "DeSantis" had a high density of mentions in tweets throughout the topic models, to voice discontent over i.e. "DeSantis' 'fascist-like' book banning spree". The mentioning of the term "nazi" and "1933" can be seen as an homage to the book burnings of the NSDAP party in Germany during and before WWII, effectively eliminating freedom of speech and expression. 


##### Red States Keywords

**Top 20 Keywords - Red States**

!['Red Top 20'](https://github.com/lydia-field/book-bans/blob/main/data_images/red_top_20.png?raw=true)

Top general keywords like “school” and “children” are also commonly used by **red states**, but mentions of “Florida” and “DeSantis” alone are notably more common in red states. Florida governor Ron DeSantis has become a bastion for the right in the book ban discussion, garnering significant media attention. Much of the discussion referencing Ron DeSantis tends to be critical, opposing his policies on book bans and censorship.


##### Red States Topic Model

**Red States Topics**

!['Red State Topics'](https://github.com/lydia-field/book-bans/blob/main/data_images/red_states_BERT.png?raw-true)

In **red states**, the most common topics, in order of coherence, are: 
1. **LGBTQ+/Pornography** (“queer”, “explicit”, “pornography”, “sexually”, “harmful”)
2. **Florida** (“florida”, “state”, “don’t”, “say”, “gay”)
3. **Race** (“black”, “white”, “racism”, history”, “supremacist”)
4. **Missouri** (“missouri”, “defund”, “libraries”)
5. **Texas** (“texas”, “texans”, “txlege”)
6. **Parents** (“parents”, “children”, “appropriate”)
7. **Moms for Liberty** (“moms”, “liberty”, “lgbtq”).

On the other hand 'red' more republican-leaning states used words such as "explicit" and "harmful" in connection to "queer". Topic Model 7 demonstrates engagement about the pro-book banning group "moms for liberty". "Trump" and "elite" was also mentioned in connection to Ron DeSantis and the book bannings, exemplifying the assertion by the opposition to book banning in red states that the Republican party ‘elite’ wants to control the narratives. Furthermore, on March 28th, 2022, DeSantis initially banned all books with gay characters, as a way to protect their children from 'obscene' works. However, Topic 11 shows that there are also various critical voices within red states, due to the frequency of "nazi", "hitler", "burned", "1933", and "repeat", viewing the above mentioned Nazi book burnings as being repeated in the form of the contemporary book bannings.


##### Blue & Red States Comparison

**Comparison** of these topics leads to the following conclusions: 

First of all, in both groups, Florida, Moms for Liberty, race and LGBTQ+ were topics of discussion, indicating that book banning in Florida, and book banning for race or LGBTQ+ reasons, are nationwide points of discussion.

However, one significant difference in the topic models is where race lied in discussion. In red states, race was one of the top three most common topics, whereas in blue states, it was the ninth most popular topic. This indicates book banning for racial reasons (inclusion of critical race theory, etc.) is a more controversial and present issue in red states than in blue ones. 

Another significance is the way that the LGBTQ+ topic was discussed between state groups. It’s important to note that, in red states, LGBTQ+ and pornography were considered in the same topic model, whereas in blue states, they were considered separately. This indicates that constituents in red states view book banning of LGBTQ+ books as book banning for pornographic reasons, whereas discussion of constituents from blue states do not tend to consider books containing LGBTQ+ material as explicit.

Another significant difference is the inclusion of “parents” as a topic model for red states, but not blue ones. This indicates that issues of parental rights in education are a more present issue for constituents of red states than blue ones. 

Both sets of states equally mentioned words related to pornography and kids, though in blue states, it was mainly used in the context to advocate for sexual education in schools, whereas in red states, the inappropriateness of such content and education being available to adolescents was heavily criticized by users such as Florida’s “moms for liberty.”


##### Blue & Red States Term Frequencies

When directly comparing two sides of a topic, term frequencies can be more illuminating than keywords alone, as they allow us to analyze the relative usage of certain words and phrases. This scattertext plot shows the comparative frequency of term usage between red and blue states, with blue states on the y-axis and red states on the x-axis. This model calculates a score for each keyword based on its frequency of usage by red states and blue states. This score determines the location and color of the data points on the plot. The distribution of the term frequency comparison between red states and blue states shows high alignment, as there are many keywords clustered in the upper right of the plot. These words have high frequency scores for both groups, indicating that there is some alignment within the discussion. 

**Red vs Blue State Relative Term Frequencies**

!['Red Blue Scattertext'](https://github.com/lydia-field/book-bans/blob/main/data_images/red_blue_scattertext.png?raw=true)

The individual terms in this cluster are not surprising, as “book” and “ban” were query keywords. However, the common frequency of “women”, “liberty”, “lgbtq”, “black history”, “abortion”, and “censorship” are more telling. (These can be seen in the interactive version of the scattertext, linked [HERE]([url](https://github.com/lydia-field/book-bans/blob/main/data_images/red_blue_scatter.html))). Although the fact that both groups use these terms at a similar frequency implies convergence within the discussion, the partisan nature of the discussion as a whole and of these terms themselves tells a different story. The implication is that book ban opponents (generally in blue states) tend to use the justifications employed by book ban supporters (generally in red states) to express their explicit opposition to such bans. Additionally, many of these keywords employed by both groups reference other contentious political discussions (like “abortion” and “lgbtq”), implying that justifications for book bans stem from other existing political controversy. 

**Top 10 Term Frequencies for Blue & Red States**

!['Top Terms'](https://github.com/lydia-field/book-bans/blob/main/data_images/top_terms_red_blue.png?raw=true)

Terms used more by one group than the other also add to this story, illuminating key lexical differences between blue state and red state discussions. In red states, much of the frequent, individual (not used often by blue states) discussion involves specific bills legislating book bans, such as Texas House Bill 900 (Dey 2023). Red state discussion also tends to include mentions of book bans in specific counties, such as Duval County in Florida. For blue states, independently frequent terms include key state political leaders, like Secretary of State Alexei Giannoulias and Governor J.B. Pritzker in Illinois.


### State case studies - Florida & California

#### Florida

Tweet Count: **5,501**

**Florida Topic Model**

!['FL topics'](https://github.com/lydia-field/book-bans/blob/main/data_images/FL_topics.png?raw=true)

The most common topics in tweets from Florida are: 
1. **Florida Republican Officials** (“Trump”, “DeSantis”, “Fascist”)
2. **Race** (“Black”, “History”, “Racist”, “White”)
3. **Antisemitism** (“Jewish”, “Hitler”, “Nazis”, “Holocaust”)
4. **Education** (“Teacher”, “Education”, “Shortage”, “Students”)
5. **Moms for Liberty** (“Moms”, “Liberty”, “Board”, “Group”).

Note: 2,949 Tweets about book banning containing 'DeSantis' alone!

**Top 20 Keywords - Florida**

!['FL words'](https://github.com/lydia-field/book-bans/blob/main/data_images/fl_top_20.png?raw=true)


#### California

Tweet Count: **1,913**

**California Topic Model**

!['CA topics'](https://github.com/lydia-field/book-bans/blob/main/data_images/ca_topics.png?raw=true)

In California, the most common topics are: 
1. **Guns** (“Guns”, “Assault”, “Weapons”, “Children”, “Shootings”, “Mass”)
2. **LGBTQ** (“Queer”, “LGBTQ”, “Gender”, “Sex”)
3. **Porn** (“Pornography”, “Sex”, “Pornographic”, “Explicit”)
4. **Florida** (“Florida”, “DeSantis”, “Maga”)

**Top 20 Keywords - California**

!['CA words'](https://github.com/lydia-field/book-bans/blob/main/data_images/ca_top_20.png?raw=true)
  

#### Florida & California Comparison

The inclusion of guns and school shootings as the most common topic in California regarding book banning is very interesting, as it indicates severely negative discussion and connotation surrounding book bans. Another important finding from this data is the presence of Florida as a top topic for both states. This is especially interesting considering the fact that California is not a common topic model for Florida, and indicates that Californian constituents are concerned with Florida’s book banning decisions, whereas Florida constituents are not concerned with California’s.


#### Florida & California Term Frequencies

**Florida & California Relative Term Frequencies**

!['FL & CA Scatter'](https://github.com/lydia-field/book-bans/blob/main/data_images/FL_CA_Scatter.png?raw=true)

The scatter text term frequency model comparing the conversations around Florida and California is very similar to the model comparing red states and blue states. This further enforces our decision to use Florida and California as case studies, and emphasizes the fact that these two states drive a significant portion of the overall partisan conversation. Like in the blue & red states models, the most frequent terms from both groups include query keywords “book” and “ban”. Unsurprisingly, California governor Gavin Newsom was frequently mentioned in the California conversation while Florida governor Ron DeSantis was frequently mentioned in the Florida conversation. “Guns”, “drag”, and “maga” were frequently used in both discussions, but slightly more so for California while “abortion”, “race”, and “lgbtw” were frequently used in both discussions, but slightly more for Florida. 

**Top 10 Term Frequencies for Florida & California**

!['Fl & CA Terms'](https://github.com/lydia-field/book-bans/blob/main/data_images/top_terms_fl_ca.png?raw=true)

Top scored keywords for California include California Superintendent of Public Instruction Tony Thurmond and discussions of “segregated campuses”. For Florida, mentions of Florida schools, Duval County, and a “book ban hoax” were the most frequent keywords. The “book ban hoax” refers to Florida governor Ron DeSantis’ statement claiming that book bans being reported in the media were a “hoax” (Friedman, 2023).


#### The 'Debate Phenomenon'

In our analysis of Florida and California, one thing that repeatedly came up was a 'Debate Phenomenon' between the state's governors, in which content would repeat with different connotations depending on the Governor mentioned. For example, one [tweet]([url](https://twitter.com/GavinNewsom/status/1660300534467944448)) that often came up featured a quote from California's Governor Newsom, where he refers to Florida's Government's actions about book banning and says: "You don't get to write history in a backroom". The ton of comments under this and similar tweets varied greatly depending on whether they mentioned Florida or California, with many constituents of California defending their governor against book bans, and many constituents of Florida defending Governor DeSantis and book banning.

In addition to debate between constituents, we also noticed debate in Tweets directly from Governors DeSantis and Newsom. Governor Newsom has posted several Tweets directly mentioning Governor DeSantis and criticizing his actions. Governor DeSantis, on the other hand, has responded to many of these Tweets, criticizing Newsom. In either case, constituents from the respective state would oftentimes flood their governor's comments with support, and flood the opposing governor's comments with criticism.

!['Gavin Tweet'](https://github.com/lydia-field/book-bans/blob/main/data_images/Gavin_tweet.png?raw=true)
!['Cali Tweet'](https://github.com/lydia-field/book-bans/blob/main/data_images/calitweet.png?raw=true)


## Conclusions

In applying this analysis to our research question, we find that partisanship, as defined by the proxy of blue states and red states, does impact the ways in which individuals discuss book bans on Twitter. Our topic models conclude that individuals in blue and red states discuss book bans in distinct ways, although there is some overlap. Where there is overlap in topic coherence and keyword frequency, red state engagers typically explain justifications and reasons for banning books, while blue state engagers use similar terms to disagree. Keyword analysis also shows that book bans in Florida commonly drive conversation across red states and blue states. Additionally, Florida governor Ron DeSantis is a key target of criticism from blue states, while California governor Gavin Newsom is a key target of criticism from red states. This implies that, on the issue of book bans and other controversial discussions, individuals are strong drivers of discussion, as it gives engagers someone to blame.


## Limitations and Avenues for Further Research

One significant limitation in our research occurs from social media algorithms. Typically speaking, individuals who utilize social media to discuss a political topic are the ones with the most passionate opinions- whether they agree or disagree with the topic. This creates a limitation in our research about the opinions of the average citizen, as our data has shown mostly Tweets of individuals who hold strong opinions about book banning. The algorithms of social media further this gap. Since social media algorithms are designed to bring attention to the most controversial and bite-worthy content, the Tweets that are more extreme tend to gain more reach, whereas less controversial Tweets gain less. This means that, even if an author with moderate opinions did post about book banning, their Tweet would be unlikely to gain as much attention, and would therefore hold less significance over the overall conversation. One way to mitigate these social media specific issues could be to supplement the data by public surveys of constituents or reviews of school board meeting transcripts. 


## Bibliography

Atterbury, A (2023, March 31), “Florida House passes parental rights bill restricting pronouns in schools”, Politico. https://www.politico.com/news/2023/03/31/florida-house-parental-rights-bill-pronouns-lgbtq-00089971

Chappell, B (2023, May 25), “1 complaint led a Florida school to restrict access to Amanda Gorman’s famous poem”, NPR News. https://www.npr.org/2023/05/24/1177877340/amanda-gorman-poem-restricted-miami-school

Dey, S (2023, April 19), “Texas House passes bill that aims to keep sexually explicit materials out of school libraries”, Texas Tribune. https://www.texastribune.org/2023/04/19/texas-libraries-books-schools-legislature/

Friedman, J (2023, June 12), “DeSantis Is Wrong. Book Bans in Florida Schools and in Other States Aren’t a ‘Hoax’”, USA Today.  https://www.usatoday.com/story/opinion/2023/06/12/book-ban-school-libraries-threat-students-education-freedom/70305740007/

Gilbert, M (2023, September 6), ‘What You Need to Know About the Book Bans Sweeping the U.S.’, Columbia University, https://www.tc.columbia.edu/articles/2023/september/what-you-need-to-know-about-the-book-bans-sweeping-the-us/. 

Harvard (2023, September 18), ‘History of Book Banning in the United States and Beyond’, Harvard University, https://guides.library.harvard.edu/c.php?g=1269000&p=9306840. 

Jason S. Kessler. Scattertext: a Browser-Based Tool for Visualizing how Corpora Differ. ACL System Demonstrations. 2017.

Meehan, K & Friedman, J (2023, April 20), “Banned in the USA: State Laws Supercharge Book Suppression in Schools”, PEN America, https://pen.org/report/banned-in-the-usa-state-laws-supercharge-book-suppression-in-schools/

Savage, C (2023, June 12), “‘First of its kind’ Illinois law will penalize libraries that ban books”, AP News. https://apnews.com/article/book-ban-library-lgbtq-illinois-f5516941473e474712eaaafda084de76

Serrano, A (2023, June 19), “Llano County libraries case has lawyers and publishers worried about existing legal precedents”, Texas Tribune. https://www.texastribune.org/2023/06/19/llano-county-books-legal/

Ukenye, L (2023, September 11), “Biden promised a book ban coordinator 3 months ago. He’s yet to name one. Politico. https://www.politico.com/news/2023/09/11/biden-book-ban-coordinator-00114993
