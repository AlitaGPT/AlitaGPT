# AlitaGPT Lite Paper: A Rational AI Model for Trading Markets
 
## From a Legendary Trader

**Question: Who is the most influential investment and trading master in modern history?**


**Buffett? Soros?**
Yet, if this question were posed to active traders, with a probability of over 80%, there would be only one answer.


**Jesse Livermore**


In 1929, he famously shorted the entire United States, prompting the White House to request him to cease; he also shorted cotton futures, turning into a legendary trader where the market could scarcely find a bale of cotton.

![微信图片_20231215123121](https://github.com/AlitaGPT/AlitaGPT/assets/153814037/0b49c74a-08c7-422f-8179-6f1cd00257dc)


His memoir, "Reminiscences of a Stock Operator," documenting his career, was published in 1940. Even after over 80 years, this book remains essential reading for successful traders. Within its pages, numerous trading strategies and principles are discussed, but prominently emphasized is the requirement for traders to counteract their innate human instincts in the midst of trading.
However, trading execution devoid of "human instincts" is precisely the advantage of AI.


<img src="![微信图片_20231215123135](https://github.com/AlitaGPT/AlitaGPT/assets/153814037/f1ee2f35-310b-49c0-9d3d-a0f64f5cabfd)" alt="![微信图片_20231215123135]" width="400" align="centre">



## 1.Training


### Patience


**Jesse Livermore**: "Only enter a trade after the action of the market confirms your opinion and then enter promptly"


Willie Alexander, the founder of AlitaGPT, was born in 1973 into an affluent family in the Upper East Side of New York, USA. At the age of 6, a car accident resulted in the amputation of his right leg. Equipped with a prosthetic limb, he often faced ridicule from classmates as the 'metallic clown.' In 1991, Willie enrolled in New York University, opting for a major in Financial Markets and Investment Analysis. Despite his introverted nature, he emerged as an expert in both finance and artificial intelligence.

Throughout his career, Willie gained a profound understanding of the complexities and risks inherent in financial markets. Recognizing the potential of applying artificial intelligence to the financial sector, he envisioned creating a brand that seamlessly integrated AI technology with financial markets. In December 2015, amid the first wave of the AI revolution, Willie's team established a project named 'Risk Aversion Vanguard' (RAV), aiming to provide users with a safer, more transparent, and intelligent financial experience through AI-assisted analysis of financial data.

On February 14, 2019, inspired after watching the movie 'Alita: Battle Angel,' Willie, a fellow 'metallic person,' rebranded the project as 'AlitaAI.' Despite not achieving a qualitative breakthrough in AI technology during the early AI era, the team endeavored to create more value and opportunities for users in the field of financial investment.

<img width="237" alt="Picture2" src="https://github.com/AlitaGPT/AlitaGPT/assets/153814037/5a46d797-51f9-45bb-a7dd-3907b3453ae5">

The release of ChatGPT in June 2012 opened a new path for AlitaAI. Leveraging the ChatGPT large model, integrating professional data and innovative algorithms accumulated by AlitaAI, the team further trained a neural network large model tailored to the financial domain. In November 2022, the LM version of AlitaAI was launched, officially rebranded as AlitaGPT.
Excerpts from 'The AlitaGPT Trilogy of Self-Iteration,'
Published in the 'ACM Transactions on Intelligent Systems and Technology'
Volume 11, Issue 1, Pages 157-160, 2023"

<img width="429" alt="Picture5" src="https://github.com/AlitaGPT/AlitaGPT/assets/153814037/97842953-cdcb-4048-93e8-718bb81c324e">

### Keep right

**Jesse Livermore**: "As long as a stock is acting right, and the market is right, do not be in a hurry to take profits"

Before its launch, AlitaGPT existed as an experimental model in the academic field, remaining untouched for commercial applications. It underwent continuous testing and self-learning with large datasets within laboratory settings. At the end of 2023, with the support of multiple prominent capital entities, the LM version of AlitaGPT went live, marking its initiation into the realms of digital currency and U.S. stock trading. 

![微信图片_20231215123141](https://github.com/AlitaGPT/AlitaGPT/assets/153814037/023712a6-cee2-4e49-adcf-f183051d53d0)


Currently, due to considerations of liquidity in the open market, this version exclusively supports U.S. stock trading and the mainstream digital currency market.
This system boasts an advanced artificial intelligence framework, possessing robust learning capabilities and intelligent analytical skills. Not only can this system comprehensively analyze complex data in financial markets, but it can also predict market trends and risks. More importantly, it offers users personalized investment advice and intelligent financial services.

## 2. Optimization

### Model Structure and Fundamental Principles

The underlying model of AlitaGPT is based on the GPT (Generative Pre-Training) model, which is built on the Transformer architecture. GPT-like models undergo unsupervised pre-training on large-scale data initially, followed by fine-tuning on smaller supervised datasets to adapt to specific tasks.
This approach of pre-training a general model and then fine-tuning for tasks does not rely on task-specific model design techniques, making it capable of achieving good performance across multiple tasks.


The GPT framework employs semi-supervised learning to accomplish language understanding tasks, dividing the training process into two stages: unsupervised pre-training and supervised fine-tuning. In the pre-training stage, a unidirectional Transformer is used to learn a language model, providing unsupervised embeddings for sentences. In the fine-tuning stage, the parameters of the Transformer are fine-tuned based on the specific task, aiming to learn a universal representation that can be adapted to various tasks with minor modifications.


GPT adopts the decoder structure of the Transformer, with some modifications. The original decoder comprises two multi-head attention structures, while GPT retains only the masked multi-head attention structure, as shown in the diagram on the right.


<img width="938" alt="Picture7" src="https://github.com/AlitaGPT/AlitaGPT/assets/153814037/1e53a997-b66c-4c01-9481-38d01972123b">

### Mission Accomplished

After extensive pre-training, for specific task objectives such as in question answering and reasoning tasks, modifications are made to the input data format, linear layer parameters are added, and vector parameters for special symbols are introduced. The diagram below illustrates the processes for four different task types. During fine-tuning for these tasks, linear layer parameters are added, along with vector parameters for special symbols such as start symbols, end symbols, and separator symbols. The model then produces task answers.


For instance, in various multiple-choice tasks, similar to question answering and reasoning tasks, background information is initially concatenated with the question. Subsequently, the concatenated text is successively combined with each answer. Finally, the concatenated text is fed into the Transformer model sequentially, and a linear layer is added at the end to predict the result of each input, completing the task.

<img width="1772" alt="Picture8" src="https://github.com/AlitaGPT/AlitaGPT/assets/153814037/cdf30aa5-1bfc-4c83-9d69-c10ff904d021">


### Financial Application of AlitaGPT

AlitaGPT focuses on the core reference indicator in the market, which is 'market sentiment.' Market sentiment encompasses the emotional response to the overall market, specific trading instruments, or even individual stocks. It represents a comprehensive display of the viewpoints of market participants and is the collective expression of feelings exhibited by all market participants. In fact, the overall trend of the current market is often determined by the mainstream perspectives of the majority of market participants. Although market sentiment does not inherently impact market prices directly, the actual operations triggered by market sentiment can directly influence prices. Since the price of any commodity depends on the supply and demand relationship, i.e., buying and selling behavior, market sentiment can induce buying and selling behaviors among market participants, thus affecting prices.


In publicly traded markets with high liquidity, market sentiment is more sensitively reflected in market performance. AlitaGPT timely and extensively collects user expressions of market sentiment and assesses the potential impact on prices based on historical trading data. This information gathering and analysis not only consider the influence of macroeconomic policies on a specific category or the direct expression of sentiment by market participants but also take into account silent considerations such as market participants' views on 'cost levels.'


For instance, when the price of an asset continues to rise, some market participants may contemplate selling a portion of their assets to realize profits or recoup investment costs. However, such actions are often not expressed through public information channels. Therefore, it is necessary to estimate the cost levels of these participants to further predict the price points at which they might sell these assets. AlitaGPT integrates these factors, continuously calculating and measuring the cost levels of market participants while extensively collecting and analyzing the sentiment expressions of market participants, to more accurately predict the potential impact on prices.


The aforementioned is the foundational logic of AlitaGPT in understanding market trends through monitoring and analyzing market sentiment, enabling it to make corresponding investment decisions. This comprehensive approach, considering market sentiment, the impact of macroeconomic policies, and cost-level factors, allows AlitaGPT to more accurately and effectively confirm market indicators and make corresponding quantitative investment actions.


![Picture6](https://github.com/AlitaGPT/AlitaGPT/assets/153814037/7a97d4d8-ec23-4f41-9606-3213bd5a7712)


### Quantitative Trading AI + Defi Vault

Vault is an essential part of the Defi ecosystem, and AlitaGPT will deploy a quantitative trading AI Defi Vault on-chain, using it as a medium to provide users with asset management services. Users can mine AlitaGPT's inscription token—AAI—by staking digital assets.


Traditional Defi Vaults rely on pre-defined arbitrage opportunities, such as on-chain lending yields or liquidity mining returns. However, with the maturation of Defi, these returns have become significantly lower. In contrast to traditional Defi Vaults, AlitaGPT Vault maintains the system mechanisms of Defi Vaults but actively seeks quantitative trading opportunities in large public markets, leveraging AI quantitative trading technology to comprehensively upgrade traditional Defi Vaults.


Furthermore, compared to users engaging in self-managed high-frequency quantitative trading, AlitaGPT Vault offers relatively lower gas fees and transaction friction costs, enabling users to achieve returns at a reduced cost. The operational process of AlitaGPT Vault is highly transparent, allowing users to clearly understand their asset status and transaction history. Additionally, AlitaGPT Vault prioritizes the security of user assets, implementing stringent security measures and a decentralized auditing mechanism to ensure the safety of users' assets. Users can confidently stake their digital assets in AlitaGPT Vault, enjoying secure, stable asset management services.


With the gradual upgrade and application of AI quantitative trading technology, AI Defi Vault emerges as a vital force within the Defi ecosystem, providing users with more robust asset management capabilities while retaining the characteristics of easy operation, optimized returns, low gas fees, transparent operations, and high security inherent in Defi Vaults.

### AAI Value Scenarios

**1.** Governance Token: AlitaGPT and its Vault platform governance are conducted through tokens. After enabling token governance, users can obtain governance tokens by staking and locking AAI tokens, based on the dimensions of quantity and time. These governance tokens will determine the voting results of all platform rights, following the principle of majority rule;


**2.** Excess Profit Distribution: AlitaGPT will continuously buy back AAI tokens in the token trading market and burn them with the quantitative investment profits obtained in different markets, ensuring the secondary market trading price of AAI;


**3.** Empowering Application Scenarios: AlitaGPT is currently deployed only in the U.S. stock and digital currency markets. According to the votes of future community users, more features will be added sequentially 

**3.1** more public market trading models, 

**3.2** real-time customized research reports for specific assets, 

**3.3** privately customized personal versions of AlitaGPT models. All these features require the consumption of AAI to provide services.

**Community70%**

**Ecology10%**

**Mechanism10%**

**Team10%**

All Supply: 2.1 Billion


Based on the BRC20 Inscription Token


Community tokens are distributed through contract staking mining;
Institutional holdings are released linearly over 12 months;
Team holdings are released linearly over 36 months.


**2023Q4**
Launch Commercialization
Deploy AlitaGPT Vault
Collaborate with MoMoChat

**2024Q22024Q42025**
Unlock more public market trading models, such as stock markets in different countries/regions, futures trading, and forex trading

**2024Q42025**
Customizable research report feature, allowing users to tailor real-time research reports for different assets at any time

**2025**
Customize AI quantitative trading or research models according to user needs; create a personalized Alita, ushering in a new era of Alita




<!--
**AlitaGPT/AlitaGPT** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
