# Assignment 2: Protests
In recent years the United States has experienced a surge of protests, in support of Black Lives Matter, gender equity, and many other social or political issues.

In this assignment, you will work with data from [Count Love](https://countlove.org/), data that is ocassionally [cited](https://www.nytimes.com/2020/08/28/us/black-lives-matter-protest.html) by the _New York Times_ when reporting on US demonstrations.

Through this assignment, you will be able to answer questions about protests, including:

* What were the most attended and least attended protests in the US in the last 5 years?
* How many protests occurred in Washington state?
* How did the number of protests in 2019 compare to 2020, and why?
* Why are people protesting in the US? What are the biggest motivators?

## Learning objectives
By completing the assignment, you will develop or skills for:

- **Version control** tools for managing code (git and GitHub)
- Writing documents with **markdown** syntax
- Coding in R
- Thinking critcally about data.

# 1. Critical Analysis & Reflection: Before You Code

Before diving into this (or any) dataset, it's important to know where the data came from, and it's important to have or to seek out _domain familiarity_ — that is, knowledge about the topic of the dataset. Sometimes the topic is very narrow; more often it is expansive, as in the case of CountLove. We don't want to be "strangers in the dataset," as Catherine D'Ignazio and Lauren Klein describe it. To get more familiar, we are going to begin by doing some background reading.

**Note:** Please write your answers below under the heading "Your Responses and Reflections."

- First, please read [this FAQ](https://countlove.org/faq.html) from the CountLove website and the opening of [this blog post](https://www.tommyleung.com/countLove/index.htm).  **(R1a)** Based on the information in these pieces, why did the creators start collecting the CountLove data?

- Next, we would like you to read this [New York Times piece that uses CountLove data](https://www.nytimes.com/interactive/2020/06/13/us/george-floyd-protests-cities-photos.html) and that describes the Black Lives Matter protests that occurred in the summer of 2020. **(R1b)** Please summarize the main point or argument of this article.

Next, we're going to reflect about who collected this data, and what's actually inside it.

**(R1c)** Who collected and shared the CountLove data, and what do they do for a living?

**(R1d)** As Klein and D'Ignazio remind us, when it comes to data, "what gets counted counts." What types of demonstrations does CountLove include in their data, and what types do they exclude?

**(R1e)** How and where does CountLove get their data about the protests?

**(R1f)** How does CountLove make their estimates about the number of people who attended a protest? What potential problems might arise from this method of estimation?

**(R1g)** What are two central values of Count Love? Name and briefly describe them. (See the Envisioning Cards for a defintion of "value".)

**(R1h)** Name and briefly describe one direct stakeholder and one indirect stakeholder (See the Envisioning Cards)?

# 2. Coding in R: Parts 1-6
**Instructions**. Assignment instructions and prompts are in this file: [analysis.R](analysis.R).

**Coding and reflection prompts**. You will find two kinds of prompts in [analysis.R](analysis.R):

* *Coding prompts*, which prompt you to write R code in [analysis.R](analysis.R).
* *Reflection prompts*, which prompt you to think and write in English below, in this file (README.md).

**Formatting Your Responses and Reflections**.

* When formatting your written responses and reflections below, please *retain* all
reflection prompt IDs (e.g., R1a, R2a, etc.).
* Fill in the elipses (...) with your own words.
* Remove expected word counts.
* To write clearly, use markdown code appropriately (e.g., **bold**, _italics_, and `code`). As appropriate, include images, links, and so forth.

**Questions?** As always, please post on Teams or ask your Instructor or Teaching Assistant.

:computer: Good coding!
   :writing_hand: Good critical thinking!
      :smile: Good-luck!

(_Updated: October 2022, Your Teaching Team_)

# 3. Critical Analysis & Reflection: After You Code

In the second chapter of *Data Feminism*, Klein and D'Ignazio describe 4 ways that data scientists can challenge power and take action:
> Taking action can itself take many forms, and in this chapter we offer four starting points:
> (1) Collect: Compiling counterdata—in the face of missing data or institutional neglect—offers a powerful starting point as we see in the example of the DGEI, or in María Salguero’s femicide maps discussed in chapter 1.
> (2) Analyze: Challenging power often requires demonstrating inequitable outcomes across groups, and new computational methods are being developed to audit opaque algorithms and hold institutions accountable.
> (3) Imagine: We cannot only focus on inequitable outcomes, because then we will never get to the root cause of injustice. In order to truly dismantle power, we have to imagine our end point not as “fairness,” but as co-liberation.
> (4) Teach: The identities of data scientists matter, so how might we engage and empower newcomers to the field in order to shift the demographics and cultivate the next generation of data feminists?

**(R1h)** How does the CountLove project embody one or more of these 4 forms of challenging power?

**(R1i)** What is the most interesting or surprising thing you learned from this analysis? Please answer in at least 2-3 sentences (2 points)

**(R1j)** What is a kind of analysis that you would like to do or that would be interesting to do with the CountLove data that you don't have the time or skills to accomplish at this moment? Please answer in at least 2-3 sentences (2 points)

## Your Responses and Reflections

### Critical Analysis & Reflection: Before You Code (questions above)

* **(R1a)** The creators initiated the collection of CountLove data with the aim of maintaining accurate records of ongoing demonstrations and enhancing public accessibility to this information. Given the multitude of protests taking place, it is all too easy to lose track of their specific locations, dates, and the number of participants, often due to institutional neglect and practical challenges.  Through the development of CountLove, the documentation and understanding of protests within the broader context of societal trends can be achieved, thereby raising public awareness and fostering a diverse, empathetic, and compassionate country.

* **(R1b)** The main point of this article is to illustrate the increasing impact of protests against discrimination faced by Blacks in the United States.

* **(R1c)** CountLove data is collected and shared by Tommy Leung and Nathan Perkins, who are engineers and scientists with a keen interest in civic responsibility and public policy.

* **(R1d)** Countlove counts public displays of protest that are not part of “regular business” as "what gets counted counts", excluding awareness events, commemorative celebrations, historic reenactments, fundraising events, townhalls, or political campaign rallies.

* **(R1e)** They get most of the data from crawling local newspaper and television sites on a daily basis, manually coding information about each protest.  They also use software to aggregate and visualize those data.

* **(R1f)** Countlove records the most conservative attendance number from the news articles that they link. They interpret “a dozen” as 10, “dozens” as 20, “hundreds” as 100, and so forth. This method of estimation might be lack of precision since converting qualitative terms to numerical estimates may not accurately represent the actual crowd size. For instance, "a dozen" could mean anywhere from 10 to 20, and "hundreds" could range from 100 to 999 which is kind of unclear.

* **(R1g)** I would say justice and dignity are two central values of Countlove. Since most protests are based on social injustices (such as racial discrimination) and the main reason for the protests is to preserve the dignity of different groups of people, collecting data about them reflect the pursuit of social justice and the desire to give dignity to the masses.

* **(R1h)**
   * Direct stakeholder: Journalists and media outlets utilize the data shared by Countlove to present their desired narratives and foster public awareness.
   * Indirect stakeholder: Readers of the newspaper and journals learned about Countlove's data indirectly, as they did not have direct access to it but were informed through alternative means.

### Part 3: Locations (`analysis.R`)
* **(R3a)** To be honest, I'm not very surprised by the number of protests in Washington. Since Washington is a highly populous and politically active region, it's not surprising to have a significant number of protests over these years.

* **(R3b)** I find the application of the sapply function to be truly fascinating. It proves to be a powerful and efficient technique for performing uniform operations on each element of a vector. This versatility makes it an invaluable tool for data analysis, and I am excited to explore its potential in future data projects.

* **(R3c)** I noticed that some of the state spellings are case sensitive, such as "te" or "wA." These are most likely input errors that occurred while collecting the data, and should be considered to merge them with the intended content if there is an opportunity to improve them.

### Critical Analysis & Reflection: After You Code (questions above)
* **(R7h)** The CountLove project mostly embodies "collect" and "teach" as a form of challenging power. Since there are many protests happened around every day, it’s easy to lose track of exactly where and when protests took place and how many people participated due to institutional neglect and practical difficulties. This project complies the data aims to keep a factual record of ongoing demonstrations and make this counterdata more accessible to the public. Additionally, Countlove is willing to be a useful source for journalists and concerned citizens, making more compelling cases for a diverse, empathetic, and kind country. It hopes to draw more attention to these protests and empower the field to change demographics and make a real difference which shows the power of "teach".

* **(R7i)**
   In this assignment, I had the opportunity to explore and enhance my data sorting skills and learned how to effectively utilize functions as powerful tools in R.  Through practical exercises, I gained valuable insights into the importance of data manipulation and analysis, and how it can lead to meaningful outcomes. Moreover, working with functions in R showcased the efficiency and convenience they bring to data analysis.  Functions allowed me to encapsulate complex operations, making the code more readable and modular.

   Overall, this assignment provided a practical foundation in data handling and demonstrated the potential of data as a transformative tool. As I continue my journey in data analysis and programming, I am excited to apply these newfound skills in various domains.

* **(R7j)** I wanted to delve deeper into the timing of these protests. I believe that the type of protest often emerges in response to a social event acting as a trigger. It seems plausible to establish a connection between the purpose of the protest and the prevailing circumstances. By identifying common patterns among these activities occurring in diverse regions simultaneously, we may gain valuable insights into the issues that genuinely matter to people.
