# Linguistic-Underpinning
Some components of this paper were conducted in ORA and R. If you need further guidance, please contact the authors. 

The detailed datasheet is presented below. 
Motivation

1. For what purpose was the dataset created? (Was there a specific task in mind? Was there a specific gap that needed to be filled? Please provide a description.)

This dataset was created to study the linguistic underpinnings of misinformation on twitter. 

2. Who created this dataset (e.g., which team, research group) and on behalf of which entity (e.g., company, institution, organization)?

This dataset was collected by Xinyu Wang. At the time of collection, Wang was a graduate student at Penn State University.

3. Who funded the creation of the dataset? (If there is an associated grant, please provide the name of the grantor and the grant name and number.)

The data was collected using free public API at the time of collection. 

4. Any other comments?

None.

Composition
1. What do the instances that comprise the dataset represent (e.g., documents, photos, people, countries)? (Are there multiple types of instances (e.g., movies, users, and ratings; people and interactions between them; nodes and edges)? Please provide a description.)

Each instance is a tweet post associated with the topic.

2. How many instances are there in total (of each type, if appropriate)?


The detailed statistics are provided in the paper. 

3. Does the dataset contain all possible instances or is it a sample (not necessarily random) of instances from a larger set? (If the dataset is a sample, then what is the larger set? Is the sample representative of the larger set (e.g., geographic coverage)? If so, please describe how this representativeness was validated/verified. If it is not representative of the larger set, please describe why not (e.g., to cover a more diverse range of instances, because instances were withheld or unavailable).)

It is a sample of all possible tweets within the time range of collection. It is intended to be representative of the discussion around the associated topic.

4. What data does each instance consist of? (``Raw'' data (e.g., unprocessed text or images)or features? In either case, please provide a description.)

Due to ethical considerations, only the tweet_ids are provided for re-hydration of the dataset. 

5. Is there a label or target associated with each instance? If so, please provide a description.

N/A

6. Is any information missing from individual instances? (If so, please provide a description, explaining why this information is missing (e.g., because it was unavailable). This does not include intentionally removed information, but might include, e.g., redacted text.)

N/A

7. Are relationships between individual instances made explicit (e.g., users' movie ratings, social network links)? ( If so, please describe how these relationships are made explicit.)

N/A

8. Are there recommended data splits (e.g., training, development/validation, testing)? (If so, please provide a description of these splits, explaining the rationale behind them.)

N/A


9. Are there any errors, sources of noise, or redundancies in the dataset? (If so, please provide a description.)

Due to the size of the data, there was no manual evaluation. We assume each tweet collected under each topic is correctly associated with that topic. 

10. Is the dataset self-contained, or does it link to or otherwise rely on external resources (e.g., websites, tweets, other datasets)? (If it links to or relies on external resources, a) are there guarantees that they will exist, and remain constant, over time; b) are there official archival versions of the complete dataset (i.e., including the external resources as they existed at the time the dataset was created); c) are there any restrictions (e.g., licenses, fees) associated with any of the external resources that might apply to a future user? Please provide descriptions of all external resources and any restrictions associated with them, as well as links or other access points, as appropriate.)

The dataset is self-contained.

11. Does the dataset contain data that might be considered confidential (e.g., data that is protected by legal privilege or by doctor-patient confidentiality, data that includes the content of individuals' non-public communications)? (If so, please provide a description.)

No; all raw data in the dataset is from public sources.

12. Does the dataset contain data that, if viewed directly, might be offensive, insulting, threatening, or might otherwise cause anxiety? (If so, please describe why.)

Since the tweets are misinformation-related, they could be offensive to some groups of people after hydration. 

13. Does the dataset relate to people? (If not, you may skip the remaining questions in this section.)

Yes, the tweets are published by social media users from Twitter.

14. Does the dataset identify any subpopulations (e.g., by age, gender)? (If so, please describe how these subpopulations are identified and provide a description of their respective distributions within the dataset.)

No.

15. Is it possible to identify individuals (i.e., one or more natural persons), either directly or indirectly (i.e., in combination with other data) from the dataset? (If so, please describe how.)

No names are directly provided. 

16. Does the dataset contain data that might be considered sensitive in any way (e.g., data that reveals racial or ethnic origins, sexual orientations, religious beliefs, political opinions or union memberships, or locations; financial or health data; biometric or genetic data; forms of government identification, such as social security numbers; criminal history)? (If so, please provide a description.)

Not in the current format. 

17. Any other comments?

None.

Collection Process

1. How was the data associated with each instance acquired? (Was the data directly observable (e.g., raw text, movie ratings), reported by subjects (e.g., survey responses), or indirectly inferred/derived from other data (e.g., part-of-speech tags, model-based guesses for age or language)? If data was reported by subjects or indirectly inferred/derived from other data, was the data validated/verified? If so, please describe how.)

The data was collected using Twitter Official API. 

2. Who was involved in the data collection process (e.g., students, crowdworkers, contractors) and how were they compensated (e.g., how much were crowdworkers paid)?

The collection was done by two graduate students. 

3. Over what timeframe was the data collected? (Does this timeframe match the creation timeframe of the data associated with the instances (e.g., recent crawl of old news articles)? If not, please describe the timeframe in which the data associated with the instances was created.)

The dataset was collected in Nov. 2021.

4. Were any ethical review processes conducted (e.g., by an institutional review board)? (If so, please provide a description of these review processes, including the outcomes, as well as a link or other access point to any supporting documentation.)

No review processes were conducted with respect to the collection and annotation of this data.

5. Does the dataset relate to people? (If not, you may skip the remaining questions in this section.)

Not in the current format of the dataset.

6. Any other comments?

None.

Preprocessing/cleaning/labeling

1. Was any preprocessing/cleaning/labeling of the data done (e.g., discretization or bucketing, tokenization, part-of-speech tagging, SIFT feature extraction, removal of instances, processing of missing values)? (If so, please provide a description. If not, you may skip the remainder of the questions in this section.)

Yes; the documents were cleaned such as removing hashtag signs.

2. Was the "raw" data saved in addition to the preprocessed/cleaned/labeled data (e.g., to support unanticipated future uses)? (If so, please provide a link or other access point to the "raw" data.)

No.

3. Is the software used to preprocess/clean/label the instances available? (If so, please provide a link or other access point.)

Yes; it is Python3.0 .

4. Any other comments?

None.

Uses

1. Has the dataset been used for any tasks already? (If so, please provide a description.)

The dataset has been used to conduct the study described in the paper. 

2. Is there a repository that links to any or all papers or systems that use the dataset? (If so, please provide a link or other access point.)

No.

3. What (other) tasks could the dataset be used for?

The dataset could possibly be used for other data analysis tasks surrounding the topics. 

4. Is there anything about the composition of the dataset or the way it was collected and preprocessed/cleaned/labeled that might impact future uses? (For example, is there anything that a future user might need to know to avoid uses that could result in unfair treatment of individuals or groups (e.g., stereotyping, quality of service issues) or other undesirable harms (e.g., financial harms, legal risks) If so, please provide a description. Is there anything a future user could do to mitigate these undesirable harms?)

No. 

5. Are there tasks for which the dataset should not be used? (If so, please provide a description.)

This dataset should not be used for spreading misinformation of any format. 

6. Any other comments?

None.

Distribution

1. Will the dataset be distributed to third parties outside of the entity (e.g., company, institution, organization) on behalf of which the dataset was created? (If so, please provide a description.)

The dataset is available for re-hydration. 

2. How will the dataset will be distributed (e.g., tarball on website, API, GitHub)? (Does the dataset have a digital object identifier (DOI)?)

The datasets containing only tweet IDs are available on this GitHub page. 

3. When will the dataset be distributed?

The dataset is distributed after the paper is published.

4. Will the dataset be distributed under a copyright or other intellectual property (IP) license, and/or under applicable terms of use (ToU)? (If so, please describe this license and/or ToU, and provide a link or other access point to, or otherwise reproduce, any relevant licensing terms or ToU, as well as any fees associated with these restrictions.)

N/A

5. Have any third parties imposed IP-based or other restrictions on the data associated with the instances? (If so, please describe these restrictions, and provide a link or other access point to, or otherwise reproduce, any relevant licensing terms, as well as any fees associated with these restrictions.)

Not to our knowledge.

6. Do any export controls or other regulatory restrictions apply to the dataset or to individual instances? (If so, please describe these restrictions, and provide a link or other access point to, or otherwise reproduce, any supporting documentation.)

Not to our knowledge.

7. Any other comments?

None.

Maintenance

1. Who is supporting/hosting/maintaining the dataset?

The first author is maintaining and hosting on github.

2. How can the owner/curator/manager of the dataset be contacted (e.g., email address)?

E-mail addresses are at the top of this document.

3. Is there an erratum? (If so, please provide a link or other access point.)

Currently, no. As errors are encountered, future versions of the dataset may be released (but will be versioned). They will all be provided in the same github location.

4. Will the dataset be updated (e.g., to correct labeling errors, add new instances, delete instances')? (If so, please describe how often, by whom, and how updates will be communicated to users (e.g., mailing list, GitHub)?)

Same as previous.

5. If the dataset relates to people, are there applicable limits on the retention of the data associated with the instances (e.g., were individuals in question told that their data would be retained for a fixed period of time and then deleted)? (If so, please describe these limits and explain how they will be enforced.)

No.

6. Will older versions of the dataset continue to be supported/hosted/maintained? (If so, please describe how. If not, please describe how its obsolescence will be communicated to users.)

Yes; all data will be versioned.

7. If others want to extend/augment/build on/contribute to the dataset, is there a mechanism for them to do so? (If so, please provide a description. Will these contributions be validated/verified? If so, please describe how. If not, why not? Is there a process for communicating/distributing these contributions to other users? If so, please provide a description.)

Errors may be submitted via the bugtracker on github. More extensive augmentations may be accepted at the authors' discretion.

8. Any other comments?

None.
