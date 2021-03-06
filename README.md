# Stylext: A Twitter Stylometry Proof of Concept
#### *Authorship Attribution and Obfuscation with Machine Learning (Scikit-Learn)*

&nbsp;

**The technical description for this project can be [read here](https://github.com/analyticascent/stylext/blob/master/Stylometric%20Analysis%20and%20Obfuscation%20Using%20Python.mdown).** 

**Context:** I began this project as a capstone for a [General Assembly course](https://generalassemb.ly/education/data-science/) I took in the spring of 2016. Work obligations (and the need to keep making minimum payments on a credit card) inhibited me from finishing the project to the level of complexity I originally intended. However, I decided to continue working on it in order to prepare myself for future data science projects/courses, and it ultimately was satisfactory enough to meet course requirements. 

It has served as useful practice for (and demonstration of) data acquisition, pre-processing, and analysis. This repository can be used to learn the basics of all three in the context of how supervised machine learning works, with respect to natural language processing in particular.

Twitter was the main target for experimental data due to the site's ease of use API, as well as to test an *assumption* online friends friends of mine had: that the 140-character post limit prevents "unique" text styles (known as *writer invariants*) from manifesting compared to more open-ended social media platforms. **This assumption turned out to be *dead* wrong.** 

The reason this hypothesis turned out to be wrong ended up being very straightforward: Due to the fact that many Twitter features thar are meant to make the most of that character limit (hashtags, emojis, retweeting, hyperlinks, etc) are *used variably* among users, the same quantity of raw text from any Twitter user can be just as distinct (if not more) than from other sites.

**Future Prospects:** The end goal with this project is a stand-alone tool that can disguise the writing style of a user while - as a possible bonus - making the text more readable to a general audience. I was inspired to develop this when pseudonymous writers in a [Freenet](https://freenetproject.org/) discussion group I frequented became aware of the work of researchers at [Drexel University on Stylometry.](https://www.cs.drexel.edu/~sa499/papers/adversarial_stylometry.pdf)

Stylext aims to be simpler to use and easier to modify than jstylo and anonymouth; both of which were the subject of complaints among those I recommended them to for not being easy to install/run/understand for laypersons. I have done my best to abide to the "don't trust what you can't comprehend" principle that some in the world of privacy tenaciously adhere to.

Anyone who is familiar with the Iris classification problem can conceptually understand how this project works. Instead of petal measurements however, average occurance of certain characters per tweet is used. More sophisticated machine learning features can be used, but simplicity is prioritized over accuracy for demonstration purposes. This should make the tool more accessible to those who intend to use it for themselves.

---

**What You Will Need to Run the Notebooks:** The bare minimum needed to run the IPython notebook (IPNB) files is the [anaconda python distribution](https://www.continuum.io/downloads) (version 3).

To work with something beyond the demo CSV files of tweets I used, you will need either the "Tweepy" python library installed or something that downloads a twitter feed in CSV form via API or web scraping (not recommended).

I will continue improving this project by experimenting with other various machine learning models and ensemble techniques. After the course, it will now go through the following stages:

* Create a time-series model that can "fingerprint" user tweet habits (potentially giving away their time zone).
* Expand the entire model to include more training features, and the feeds of all US senators and representatives.
* Continue improving the accuracy over time while also developing ways of subverting those same techniques as well.

There are numerous ways of defining ideal accuracy and a near infinite number of ways of combining various features in various model approaches. This will be an open-ended project that I intend to continue improving until I get too occupied with other things. That likely will not be an issue until next year, maybe.

#### Stages Executed for Project Completion:

* Acquire Tweets using a Tweepy API script
* "Fingerprint" feeds using Ipython notebook
* Use machine learning for Tweet attribution

#### Ongoing Experimentation You May Want to Try:

* Different Twitter datasets
* Varied choice of features
* Other attribution models

New development from yours truly will cease altogether when (a) time put into it gives diminishing accuracy returns, and (b) other projects begin taking up the bulk of my time. Not so unusual of a set of benchmarks now is it? 
