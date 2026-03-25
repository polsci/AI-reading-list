# AI Reading List

[Geoff Ford](https://geoffford.nz/)

This reading list is intended for students in ARTS102 and DIGI405. I will update it from time to time with interesting articles on different aspects of generative AI. If you are a student in ARTS/DIGI, feel free to email me with suggested reading to add here.  

I've released this on Github in case it is useful to others.  

The focus here is on understanding the output of large language models (LLMs) and some of the key problems with the technology. The focus on problems or limitations is intentional. There is no shortage of hype about gen AI and its claimed benefits for society, including "learners". You will have no problem finding sources, including academic research, from this perspective.  

**For students in ARTS102**, you should note that some of the sources below have not been through a process of peer review. In some cases, that is because the work is intended for a non-academic audience. In other cases, this is more to do with publishing practices in the specific field. Research on LLMs and generative AI is often released as preprints prior to submission to a peer-reviewed journal. In some cases research is published in the proceedings of conferences and papers undergo a process of peer review before being published. In some cases the research will never undergo traditional peer review, but you will find discussion and critique in work that cites them if they become influential.   

There are readings related to the following:  

* [Introduction to LLMs](#introduction-to-llms)  
* [LLMs hallucinations, bullshit, and what LLMs know](#user-content-llms-hallucinations-bullshit-and-what-llms-know)  
* [Hallucinated evidence](#hallucinated-evidence)  
* [Bias](#bias)  
* [Sycophancy](#sycophancy)  
* [Training data](#training-data)  
* [Understanding system prompts](#understanding-system-prompts)  
* [Environmental impact](#environmental-impact)  
* [Human impact](#human-impact)  
* [Hacking LLMs](#hacking-llms)  
* [Generated images and video](https://github.com/polsci/AI-reading-list#generated-images-and-video)  

## Introduction to LLMs    

These are links that LLMs and how they work as probabilistic next word predictors. The "Stochastic Parrots" article introduces some of the big issues, including environmental costs, the problems with massive data-sets of scraped data sourced from the internet (e.g. bias, baking in "hegemonic worldviews"), and points out a disconnect between parroting language and "understanding". Doctorow, a sci-fi author and tech activist, frames LLMs as "plausible sentence generators". Finally, there is an article that discusses the tendency to anthropomorphize generative AI, and some ways to avoid this.  

* [Wolfram, S. (2023). "What Is ChatGPT Doing and Why Does It Work?"](https://writings.stephenwolfram.com/2023/02/what-is-chatgpt-doing-and-why-does-it-work/)  
* [Bender, E. M., et al. (2021). "On the Dangers of Stochastic Parrots: Can Language Models Be Too Big?"](https://dl.acm.org/doi/10.1145/3442188.3445922)  
* [Doctorow "Plausible sentence generators"](https://locusmag.com/feature/commentary-by-cory-doctorow-plausible-sentence-generators/)  
* [De-anthropomorphizing “AI”: From wishful mnemonics to accurate nomenclature ](https://firstmonday.org/ojs/index.php/fm/article/view/14366)  

## LLMs hallucinations, bullshit, and what LLMs know  

Through training to be next word predictors, LLMs learn a representation of language that encodes knowledge about the world. This can be factual, human beliefs and biases, frequent associations, and so on. While it is possible to get accurate claims from an LLM, a key issue with LLMs is their tendency to "hallucinate", or make things up, expressing this "bullshit" (i.e. information communicated without regard for truth) in a plausible way that can fool the user.   

* [ChatGPT is a blurry jpeg of the web](https://web.archive.org/web/20230228010910/https://www.newyorker.com/tech/annals-of-technology/chatgpt-is-a-blurry-jpeg-of-the-web)  
* [Survey of Hallucination in Natural Language Generation](https://dl.acm.org/doi/10.1145/3571730)  
* [A Survey on Hallucination in Large Language Models: Principles, Taxonomy, Challenges, and Open Questions](https://arxiv.org/pdf/2311.05232)  
* [Hicks, M. T., et al. (2024). "ChatGPT is Bullshit."](https://link.springer.com/article/10.1007/s10676-024-09775-5)  
* [New sources of inaccuracy? A conceptual framework for studying AI hallucinations](https://misinforeview.hks.harvard.edu/article/new-sources-of-inaccuracy-a-conceptual-framework-for-studying-ai-hallucinations/)  
* [What do large language models know?](https://www.cambridge.org/core/journals/philosophy-of-science/article/what-do-large-language-models-know-tacit-knowledge-as-a-potential-causalexplanatory-structure/9475F1504081116099098C37D6F57611)

## Hallucinated evidence  

A specific class of hallucination that is relevant to student work is the hallucination of citations, or evidence more broadly. While some LLM-based chatbots increasingly access internet sources directly at the time they generate answers, they are still prone to make up sources, make up claims about sources, or just decorate their next-word-predicted claims with a web sources of varying quality. These articles/links address this issue, the varying performance of different chatbots, and some high profile examples of real-world use of hallucinated evidence.  

* [Fabrication and errors in the bibliographic citations generated by ChatGPT](https://www.nature.com/articles/s41598-023-41032-5)  
* [Hallucinated citations produced by generative artificial intelligence may constitute research misconduct when citations function as data in scholarly papers](https://www.tandfonline.com/doi/full/10.1080/08989621.2026.2645390#d1e218)  
* [Cabezas-Clavijo & Sidorenko-Bautista (2025) "Assessing the performance of 8 AI chatbots in bibliographic reference retrieval"](https://arxiv.org/abs/2505.18059)  
* [AI Hallucination Legal Cases](https://www.damiencharlotin.com/hallucinations/)  
* [Deloitte to pay money back to Albanese government after using AI in $440,000 report](https://www.theguardian.com/australia-news/2025/oct/06/deloitte-to-pay-money-back-to-albanese-government-after-using-ai-in-440000-report)  

## Bias

Research on a previous generation of language models (word embeddings) demonstrated stereotypes related to gender and ethnicity learned from the huge amount of text used in training. Texts about the world, written by real people, reflect real-world prejudice. Modern LLMs, while more complex, demonstrate similar social biases and stereotypes despite attempts by people producing them to prevent obvious bias. This matters, because LLMs are already used in systems that evaluate people. I've also included a link to an article examining cognitive biases in LLMs normally associated with human thinking.  

* [Word embeddings quantify 100 years of gender and ethnic stereotypes](https://www.pnas.org/doi/10.1073/pnas.1720347115)
* [Marked personas: Using natural language prompts to measure stereotypes in language models](https://aclanthology.org/2023.acl-long.84.pdf)
* [Explicitly unbiased large language models still form biased associations](https://pmc.ncbi.nlm.nih.gov/articles/PMC11874501/)  
* [(Ir)rationality and cognitive biases in large language models](https://royalsocietypublishing.org/rsos/article/11/6/240255/66476/Ir-rationality-and-cognitive-biases-in-large)  

## Sycophancy

Users of LLM-based chatbots note their helpfulness, agreeableness, or sycophancy. The first article below connects this to training LLMs on human feedback. The second, is an older study that is relevant to understand the impact of flattery on human users. The final article from the American Psychological Association discusses some of the psychological impacts of sycophancy (and other aspects of emotional connection) on people using AI chatbots.  

* [How RLHF Amplifies Sycophancy](https://arxiv.org/abs/2602.01002)  
* [Silicon sycophants: the effects of computers that flatter](https://www.sciencedirect.com/science/article/pii/S1071581996901044?via%3Dihub) [PDF](https://pdfs.semanticscholar.org/5545/8ec25f12b1aa7b038f1352a5e8503822574a.pdf) 
* [AI chatbots and digital companions are reshaping emotional connection](https://www.apa.org/monitor/2026/01-02/trends-digital-ai-relationships-emotional-connection)  

## Training data

The "Stochastic Parrots" paper above is a good starting point on some of the issues with massive text data used to train LLMs. Below I've linked to some interesting work from Mozilla on one data-set used in training LLMs. I've also included a link to Te Mana Raraunga | Māori Data Sovereignty Network on AI and algorithms, which includes discussion of how Māori data is collected and used.  

* [Training Data for the Price of a Sandwich: Common Crawl's Impact on Generative AI](https://www.mozillafoundation.org/en/research/library/generative-ai-training-data/common-crawl/)  
* [Indigenous Data Sovereignty, AI & Algorithms](https://www.temanararaunga.maori.nz/indigenous-data-sovereignty-ai-algorithms)  

## Understanding system prompts

System prompts are hidden prompts implemented in a LLM-based system (e.g. a chatbot) that guides how the LLM should respond to the user. Leaks of system prompts provide insight into the persona intended by AI platforms for chatbots and other systems. I haven't found academic research that digs into system prompts, but the second article provides analysis of the content and composition of system prompts. I agree with their conclusion: "System Prompts Deserve More Attention".  

* Leaked system prompts on Github: [CL4R1T4S](https://github.com/elder-plinius/CL4R1T4S) or [leaked-system-prompts](https://github.com/jujumilk3/leaked-system-prompts)  
* [How System Prompts Define Agent Behavior](https://www.dbreunig.com/2026/02/10/system-prompts-define-the-agent-as-much-as-the-model.html)  

## Environmental impact

A key issue in the take-up of generative AI systems is the environmental impact of training new generative AI models and deploying them for widespread use.    

* [Explained: Generative AI’s environmental impact](https://news.mit.edu/2025/explained-generative-ai-environmental-impact-0117)  
* ["A.I. Is on the Rise, and So Is the Environmental Impact of the Data Centers That Drive It"](https://www.smithsonianmag.com/science-nature/with-ai-on-the-rise-what-will-be-the-environmental-impacts-of-data-centers-180987379/)  

## Human impact

LLMs are made by people and used by people. These links provide examples of human harms associated with the production of LLMs and the use of AI.  

* ["OpenAI Used Kenyan Workers on Less Than $2 Per Hour to Make ChatGPT Less Toxic"](https://time.com/6247678/openai-chatgpt-kenya-workers/)  
* [Artificial intelligence and adolescent well-being: an APA health advisory](https://www.apa.org/topics/artificial-intelligence-machine-learning/health-advisory-ai-adolescent-well-being)  

## Hacking LLMs

LLMs are trained to follow instructions, but this makes it difficult to secure LLM-based systems. Generative AI's succeptibility to prompt injection and other vulnerabilities is an issue I want students to know about. We can understand "hacking AI" in a broader sense beyond illegality and malice (I'm not advocating either) and define "hacking" in a more open way as manipulation of LLMs as a component in technological system. Understanding that LLM-based systems are prone to manipulation/hacking through natural language:  

1. balances our perception of generative AI as "smart", aligned with progress, and generally surpassing human capabilities;  
2. helps us remember that humans are creative and intelligent;  
3. helps us recognise LLM-based systems are technological systems with limitations;    
4. allows us to think more broadly about the possibility that individuals and collectives can resist and oppose harmful AI systems pointed at us.  

The links below discuss prompt injection and other vulnerabilities of LLMs, including the ability to poison training data with a few samples. 

* [Video: Ways to Attack LLMs: AI Vulnerabilities exposed](https://www.youtube.com/watch?v=gUNXZMcd2jU)  
* [2025 Top 10 Risk and Mitigations for LLMs and Gen AI Apps](https://genai.owasp.org/llm-top-10/)   
* [A small number of samples can poison LLMs of any size](https://www.anthropic.com/research/small-samples-poison)  
* [Not What You've Signed Up For: Compromising Real-World LLM-Integrated Applications with Indirect Prompt Injection](https://dl.acm.org/doi/10.1145/3605764.3623985)   
* [8 Real World Incidents](https://prompt.security/blog/8-real-world-incidents-related-to-ai)  

## Generated images and video

I will add some more links here at some point, but this is an interesting read for now:  

* [How to read an AI image](https://cyberneticforests.substack.com/p/how-to-read-an-ai-image)  

