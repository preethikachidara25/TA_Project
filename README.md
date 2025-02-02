# TA_Project


#### Informational Characteristics

question="""Evaluate the video ad based on the following criteria and provide responses strictly in this format and output should be only dictionary with no prefixes:

Logical Reasoning: Rate the extent to which the ad uses logical reasoning to persuade the viewer on a scale of 1 to 5, where 1 means "very weak" and 5 means "very strong."
Factual Claims: Rate the extent to which the ad makes factual claims about the product on a scale of 1 to 5, where 1 means "very weak" and 5 means "very strong."
Functional Benefits: Rate the extent to which the ad identifies functional benefits of the product to the user on a scale of 1 to 5, where 1 means "very weak" and 5 means "very strong."
New Product Introduction: Indicate whether the ad is introducing a new product or service:
0 = Not a new product/service
1 = New product/service
Price Level: Classify the product's price level:
1 = Low-priced (consumer packaged goods)
2 = Moderately priced (consumer electronics)
3 = High-priced (automobiles)
For each criterion, provide a brief explanation in quotes for your rating.


Logical Reasoning: [Rating (1-5), reason]
Factual Claims: [Rating (1-5), reason]
Functional Benefits: [Rating (1-5), reason]
New Product Introduction: [Indicator(0-1)]
Price Level: [Level (1-3)]

Do not add any prefix word or symbol before output and output should be just like following example Response without any braces { or }

"Logical Reasoning": [4, "The ad effectively uses deductive reasoning to connect the product's features to its benefits."]
"Factual Claims": [3, "The ad makes specific claims about the product's performance, but lacks concrete evidence."]
"Functional Benefits": [5, "The ad clearly highlights the product's key benefits and how they solve consumer problems."]
"New Product Introduction": 0
"Price Level": 2


#### Emotional Characterisitics

 """
 question="""Evaluate the video content based on the following emotional criteria and provide responses strictly in this format and output should be only list with no prefixes:

Rate the extent to which the ad evokes each of the following emotions on a scale of 1 to 5, where 1 means "very weak" and 5 means "very strong." and also provide What are other emotions aroused by the ad in the last element of the list in single quotes

For each score, provide a brief explanation (reason) separated by quotes for your rating.

Love: [score (1-5), reason]
Pride: [score (1-5), reason]
Courage: [score (1-5), reason]
Joy: [score (1-5), reason]
Triumph: [score (1-5), reason]
Warmth: [score (1-5), reason]
Excitement: [score (1-5), reason]
Sadness: [score (1-5), reason]
Shame: [score (1-5), reason]
Fear: [score (1-5), reason]
Humor: [score (1-5), reason]
Anger: [score (1-5), reason]
Disgust: [score (1-5), reason]
Hatred: [score (1-5), reason]
Deprivation: [score (1-5), reason]
Failure: [score (1-5), reason]
Guilt: [score (1-5), reason]
Nostalgia: [score (1-5), reason]
Erotic: [score (1-5), reason]
Other Emotions: [list of other emotions]
Example:

{
  "Love": [3, "The ad evokes a sense of fondness for the brand, but it doesn't create deep emotional connections."],
  "Pride": [1, "The ad doesn't inspire feelings of national pride or personal accomplishment."],
  "Courage": [2, "While there are hints of overcoming challenges, the ad doesn't focus on acts of bravery."],
  "Joy": [4, "The upbeat music and cheerful visuals create a sense of happiness and lightheartedness."],
  "Triumph": [2, "The ad doesn't highlight significant victories or achievements."],
  "Warmth": [3, "The ad creates a sense of comfort and familiarity, but it doesn't evoke strong feelings of affection."],
  "Excitement": [4, "The fast-paced editing and dynamic visuals generate a sense of anticipation and energy."],
  "Sadness": [1, "The ad doesn't aim to induce sadness or melancholy."],
  "Shame": [1, "The ad doesn't evoke feelings of embarrassment or guilt."],
  "Fear": [1, "The ad doesn't induce fear or anxiety."],
  "Humor": [5, "The witty dialogue and humorous situations create a strong sense of amusement."],
  "Anger": [1, "The ad doesn't provoke anger or frustration."],
  "Disgust": [1, "The ad doesn't evoke feelings of revulsion or distaste."],
  "Hatred": [1, "The ad doesn't induce hatred or animosity."],
  "Deprivation": [1, "The ad doesn't evoke feelings of longing or want."],
  "Failure": [1, "The ad doesn't focus on failure or disappointment."],
  "Guilt": [1, "The ad doesn't induce guilt or remorse."],
  "Nostalgia": [2, "The ad evokes mild nostalgia, but it doesn't rely heavily on sentimental memories."],
  "Erotic": [1, "The ad doesn't have any sexual content or innuendo."],
  "Other Emotions": ["Surprise, Intrigue"]
} """



#### Surprise Characteristics

question="""Evaluate the video ad based on the following criteria and provide responses strictly in this format and output should be only dictionary with no prefixes:

For each driver, provide a score (1-5) and a brief explanation for the rating:

Surprise: [Rate the level of surprise evoked by the ad, reason]
Suspense: [Rate the level of suspense created by the ad, reason]
Drama: [Rate the level of dramatic impact in the ad, reason]
Narrative: [Rate the strength and coherence of the narrative, reason]
Character: [Rate the development and relatability of the characters, reason]
Plot: [Rate the engagement and coherence of the plot, reason]
Sex: [Rate the level of sexual content in the ad, reason]

For each criterion, provide a rating and brief explanation in quotes for your rating. Do not add any prefix word or symbol before output and output should be just like following example Response without any braces { or }

Example:

"Surprise": [3, "The ad uses unexpected twists and turns to create a moderate level of surprise."]
"Suspense": [2, "While there are some moments of uncertainty, the overall pace is relatively slow."]
"Drama": [4, "The ad effectively uses dramatic elements to heighten emotional impact."]
"Narrative": [5, "The narrative is well-structured and engaging, with a clear beginning, middle, and end."]
"Character": [3, "The characters are somewhat relatable but lack depth and development."]
"Plot": [4, "The plot is coherent and keeps the viewer interested."]
"Sex": [1, "The ad contains no explicit sexual content."]

"""

#### Special Characters

question="""Evaluate the video ad based on the following criteria and provide responses strictly in this format and output should be only dictionary with no prefixes:

Evaluate the video content for the presence of the following special elements and provide responses strictly in this format/examples provided below

Baby: Does the ad feature a baby? (0 = No, 1 = Yes)
Animal: Does the ad feature an animal? (0 = No, 1 = Yes)
Cartoon: Does the ad use cartoon characters or animation? (0 = No, 1 = Yes)
Celebrity: Does the ad feature a celebrity? (0 = No, 1 = Yes)"
Does the product only appear at the end of the commercial story? (0 indicates the absence,  1 indicates the presence)
Does the commercial show/mention the name of, or show the logo of a competitor, or compare the current product with an older version? (0 indicates the absence, 1 indicates the presence)
Animal_type: If ad features an animal, what animal is featured? Provide a text(Eg: Dog)

 Output should follow the Example Response provided below:

Baby: 0
Animal: 1
Cartoon: 1
Celebrity: 0
Product_only_appear_at_the_end: 1
Commercial_mention_the_name: 0
Animal_type: 'Cat'


"""

#### Celebrity Characterisitics

question="""Evaluate the video ad based on the following criteria and provide responses strictly in this format and output should be only dictionary with no prefixes:

Evaluate the video content for the presence of the following special elements and provide responses strictly in this format/examples provided below - Output should be just the list:

Sport: Is the celebrity in the ad related to sport(0 = No, 1 = Yes),reason for the answer]
Movie: Is the celebrity in the ad related to movie(0 = No, 1 = Yes),reason for the answer]
Politician: Is the celebrity in the ad related to politics(0 = No, 1 = Yes),reason for the answer]
Singer: Is the celebrity in the ad a singer(0 = No, 1 = Yes),reason for the answer]
Credibility:Is the celebrity credible? (1 = Not at all, 5 = Very much),reason for the answer]
Trustworthiness: Is celebrity trustworthy?(1 = Not at all, 5 = Very much),reason for the answer]
Physical Attractiveness: Is celebrity physically attractive? (1 = Not at all, 5 = Very much),reason for the answer]
Popularity: Is celebrity popular?(1 = Not at all, 5 = Very much),reason for the answer]
Product Knowledge: Is celebrity Knowledgeable about the product?((1 = Not at all, 5 = Very much),reason for the answer]
Product Fit: Does celebrity have a good fit with the product?((1 = Not at all, 5 = Very much),reason for the answer]
Name: Name of the celebrity in the video


For each criterion, provide a answer and brief explanation in quotes for your answer. Do not add any prefix word or symbol or word "json" before output and output should be just like following example Response without any braces { or }

Example for above format. Output should be strictly in below format with no prefixes and just the output: 
"Sport": [0, "The celebrity is not a professional athlete or known for sports-related activities."]
"Movie": [1, "The celebrity is a well-known actor who has appeared in numerous movies."]
"Politician": [0, "The celebrity is not a politician or involved in politics."]
"Singer": [0, "The celebrity is not a professional singer or musician."]
"Credibility": [4, "The celebrity has a strong and positive image that aligns well with the product's brand."]
"Trustworthiness": [4, "The celebrity is perceived as honest and reliable, making them a trustworthy endorser."]
"Physical Attractiveness": [5, "The celebrity is highly attractive and has a strong visual appeal."]
"Popularity": [5, "The celebrity is widely recognized and admired by the target audience."]
"Product Knowledge": [3, "The celebrity seems to have a basic understanding of the product's features."]
"Product Fit": [4, "The celebrity's image and personality complement the product's brand image."]
"Name": "John Doe"


If there is no celebrity in the ad, provide following response

"Sport": [0, "No celebrity is featured in the ad."]
"Movie": [0, "No celebrity is featured in the ad."]
"Politician": [0, "No celebrity is featured in the ad."]
"Singer": [0, "No celebrity is featured in the ad."]
"Credibility": [0, "Not applicable, as no celebrity is featured."]
"Trustworthiness": [0, "Not applicable, as no celebrity is featured."]
"Physical Attractiveness": [0, "Not applicable, as no celebrity is featured."]
"Popularity": [0, "Not applicable, as no celebrity is featured."]
"Product Knowledge": [0, "Not applicable, as no celebrity is featured."]
"Product Fit": [0, "Not applicable, as no celebrity is featured."]
"Name": "None"
"""

#### Price Level Characteristics

question="""Evaluate the video ad based on the following criteria and provide responses strictly in this format and output should be only dictionary with no prefixes:

For each criterion, provide a answer and brief explanation in quotes for your answer. Do not add any prefix word or symbol or word "json" before output and output should be just like following example Response without any braces { or }

Criteria:

Price Level:

Classify the product's price level:
1 = Low-priced (consumer packaged goods)
2 = Moderately priced (consumer electronics)
3 = High-priced (automobiles)
Promotional Offers:

Does the ad mention a cash back, rebate, sale, or promotion? (0 = No, 1 = Yes)

Does the commercial announce a special sales event, rebate for a limited time, or special deals? (0 = No, 1 = Yes)

Social Responsibility:
Rate the extent to which the ad highlights the company's commitment to social responsibility, such as environmental sustainability or social causes, on a scale of 1 to 5.

Example for above format. Output should be strictly in below format with no prefixes and just the output: 

"Price Level": [2, "The product is a moderately priced consumer electronic."],
"Promotional Offers": [1, "The ad mentions a 10% cashback offer for a limited time."],
"Special Sales Events": [1, "The commercial announces a special Black Friday sale."],
"Social Responsibility": [3, "The ad mentions the company's commitment to sustainable practices and reducing its carbon footprint."]"""

#### Video Characterisitics

question="""
Evaluate the video ad based on the following criteria and provide a response in a dictionary format.

For each criterion, provide a list containing:

Score: 0 or 1
Reason: A brief explanation for the score
Criteria:

Video Length (seconds): Total duration of the ad in seconds.
Slipstreaming: Is the ad related to a contemporary event?
Sex Appeal: Does the ad contain sexual appeals?
Call to Action: Is the viewer explicitly urged to take action after the commercial?
Excitement Appeal: Is excitement, new sensations, or avoiding boredom a major focus?
Self-Esteem Appeal: Is feeling better about oneself, improving oneself, or being a better person a major focus?
Achievement/Status Appeal: Is superiority, getting ahead, winning, or being better than others a major focus?
Social Appeal: Is social approval, belonging, or winning friends a major focus?
Welfare/Philanthropic Appeal: Is caring or providing for others a major focus (e.g., environment, charity)?
Nature Appeal: Does the commercial show strikingly beautiful scenes of nature?
Character Appeal: Does the commercial present a strikingly beautiful or ugly character?

For each criterion, provide a answer and brief explanation in quotes for your answer. Do not add any prefix word or symbol ``` or word "json" before output and output should be just like following example Response without any braces { or }

Example for above format. Output should be strictly in below format with no prefixes and just the output: 

"Video Length": [30, "The ad is 30 seconds long."],
"Slipstreaming": [0, "The ad is not related to a current event."],
"Sex Appeal": [1, "The ad contains suggestive imagery."],
"Call to Action": [1, "Viewers are encouraged to visit the website for more information."],
"Excitement Appeal": [1, "The ad emphasizes excitement and novelty."],
"Self-Esteem Appeal": [0, "The ad does not focus on self-improvement or personal growth."],
"Achievement/Status Appeal": [1, "The ad highlights the idea of achieving success and status."],
"Social Appeal": [0, "Social approval is not a major theme of the ad."],
"Welfare/Philanthropic Appeal": [0, "The ad does not focus on social or environmental issues."],
"Nature Appeal": [1, "The ad features stunning nature scenes."],
"Character Appeal": [1, "The ad features a strikingly beautiful character."]

"""

#### Audio and Voice Characterisitics

question="""
Evaluate the video ad based on the following sound and audio criteria and provide responses strictly in this format:

Output: A dictionary with lists, where each list contains a value or a range, and a brief explanation for the value or range.

Criteria:

Unusual Sound Effects: Rate the presence of unusual or out-of-place sound effects on a scale of 1 to 5 (1 = very weak, 5 = very strong).
Music Presence: Is music present in any form? (0 = No, 1 = Yes)
Music Type: Describe the type of music used in the ad (e.g., pop, rock, classical).
Music Popularity: Rate the popularity of the music on a scale of 1 to 5 (1 = not at all popular, 5 = very popular).
Music-Product Relevance: Does the music contain a message related to the product? (0 = No, 1 = Yes)
Beats Per Minute (BPM): Estimate the average BPM of the background music.
Music Key: Indicate the key of the background music (e.g., major, minor, or other).
Average Pitch of Voice: Calculate the average pitch of the voice in the ad (in Hertz).
Standard Deviation of Voice Pitch: Calculate the standard deviation of the voice pitch in the ad (in Hertz).
Average Intensity of Voice: Calculate the average intensity of the voice in the ad (in decibels).
Average Harmonics-to-Noise Ratio of Voice: Calculate the average harmonics-to-noise ratio of the voice in the ad.


For each criterion, provide a answer and brief explanation in quotes for criterias for your answer. Do not add any prefix word or symbol ``` or word "json" before output and output should be just like following example Response without any braces { or }

Example for above format. Output should be strictly in below format with no prefixes and just in following format: 
"Unusual Sound Effects": [2, "There are a few sound effects, but they are subtle and well-integrated."],
"Music Presence": [1, "Yes, background music is used throughout the ad."],
"Music Popularity": [4, "The music is a popular song from a well-known artist."],
"Music-Product Relevance": [0, "The music does not directly relate to the product or its message."],
"Music Type": ["Pop","Reason for the Music Type"],
"BPM": [120, "Reason for the providing respective BPM"], 
"Music Key": ["Major","Reason"],
"Average Pitch of Voice": [150,"Reason"],
"Standard Deviation of Voice Pitch": [10,"Reason"],
"Average Intensity of Voice": [65,"Reason"],
"Average Harmonics-to-Noise Ratio of Voice": [15,"Explanation"]

"""

#### Cast Characterisitics


question="""Analyze the commercial video and provide the following information:

Is there a principal character in the commercial? (0 = No, 1 = Yes)
What is the gender of the principal character? (Male = 0, Female =1, Non-binary =2)
Is the principal character a child or an adult? (Child =0, Adult =1)
What is the ethnicity of the principal character? (White = 0, Black  =1, Asian =2, Hispanic =3, other minority = 4)
Is the principal character a cartoon or created figure (e.g., Ronald McDonald)? (0 = No, 1 = Yes)
Are there any minor roles played by Asian, Black, Hispanic, or other minority characters? (0 = No, 1 = Yes)
Are there any minor roles played by animals? (0 = No, 1 = Yes)
Are there any minor roles played by cartoons or created figures? (0 = No, 1 = Yes)
What is the diversity of the cast (feature characters from various ethnicities)? (1-5, where 1=Not at all and 5=Very much)

For each criterion, provide just the answer Do not add any prefix word or symbol ``` or word "json" before output and output should be just like following example Response without any braces { or } or commna. There should not be any comma between the lines

Example shown below

"Is there a principal character in the commercial?": 1
"What is the gender of the principal character?": 1
"Is the principal character a child or an adult?": 0
"What is the ethnicity of the principal character?": 2
"Is the principal character a cartoon or created figure (e.g., Ronald McDonald)?": 0
"Are there any minor roles played by Asian, Black, Hispanic, or other minority characters?": 1
"Are there any minor roles played by animals?": 0
"Are there any minor roles played by cartoons or created figures?": 0
"What is the diversity of the cast (feature characters from various ethnicities)?": 3

"""

#### Video Format

question="""
Evaluate the video ad based on the following criteria and provide a response in a dictionary format.

For each criterion,  provide a score (1-5) and a brief explanation for the rating::

Criteria:

Testimonial: [Rating (1-5), "Reason for rating"]
Comedy: [Rating (1-5), "Reason for rating"]
Serious Drama: [Rating (1-5), "Reason for rating"]
Fantasy: [Rating (1-5), "Reason for rating"]
Animation/Cartoon: [Rating (1-5), "Reason for rating"]
Type of Product: [Provide a brief response on what Product Type is promoted in the ad]

For each criterion, provide a answer and brief explanation in quotes for your answer. Do not add any prefix word or symbol ``` or word "json" before output and output should be just like following example Response without any braces { or }

Example for above format. Output should be strictly in below format with no prefixes and just the output: 

"Testimonial": [3, "The ad features a few customer testimonials, but they are not the primary focus."],
"Comedy": [1, "The commercial is not intended to be funny."],
"Serious Drama": [2, "There are elements of emotional storytelling, but it's not overly dramatic."],
"Fantasy": [0, "The commercial presents a realistic scenario."],
"Animation/Cartoon": [0, "The commercial is entirely live-action."],
"Type of Product": ["Skincare Cream"]

"""

#### Commercial Characteristics

question="""Analyze the commercial video and provide the following information:

Analyze the commercial video and provide the following information:

Location:
1 = none,
2 = early,
3 = middle,
4 = end,
5 = intermittent (if the brand name appeared in multiple places in the ad).
[Rating (1-5)]
Brand Display Duration:
What is the total time the brand name/logo was displayed in the ad? [Time]
Brand Discussion Duration:
What is the total time the brand was mentioned in the ad? [Time]
Surprise Location:
Where in the ad does the surprising outcome occur?
1 = no element,
2 = at beginning,
3 = at middle,
4 = at end,
5 = throughout
[Rating (1-5)]
Blind Lead:
Does the product only appear at the end of the commercial story?
Binary Scale (0 indicates the absence or 1 indicates the presence)
[Rating (0 or 1)]


For each criterion, provide just the answer Do not add any prefix word or symbol ``` or word "json" before output and output should be just like following example Response without any braces { or } or commna. There should not be any comma between the lines

Example shown below

"Location": 3
"Brand Display Duration 1": "5 seconds"
"Brand Discussion Duration 2": "10 seconds"
"Surprise Location": 4
"Blind Lead": 0

"""

#### General Impression Question

question="""Analyze the commercial video and provide the following information:

Analyze the commercial video and provide the following information:

1.	Logical Reasoning: Rate the extent to which the ad uses logical reasoning to persuade the viewer on a scale of 1 to 5, where 1 means "very weak" and 5 means "very strong."

2.	Factual Claims: Rate the extent to which the ad makes factual claims about the product on a scale of 1 to 5, where 1 means "very weak" and 5 means "very strong."

3.	Functional Benefits: Rate the extent to which the ad identifies functional benefits of the product to the user on a scale of 1 to 5, where 1 means "very weak" and 5 means "very strong."

4.	New Product Introduction: Indicate whether the ad is introducing a new product or service: 0 = Not a new product/service 1 = New product/service

For each criterion, provide just the answer Do not add any prefix word or symbol ``` or word "json" before output and output should be just like following example Response without any braces { or } or commna. There should not be any comma between the lines

Example shown below

"Logical Reasoning:": 3
"Factual Claims": "5"
"Functional Benefits": "1"
"New Product Introduction": 1

"""

#### Brand Questions

question="""Analyze the commercial video and provide the following information:

Brand:
1.	Are consumers familiar with the advertised brand? (1= Not at all, 5 = very much)
2.	Is the advertised brand very popular with consumers? (1= Not at all, 5 = very much)
3.	Is the advertised brand perceived to have high quality? (1= Not at all, 5 = very much)
4.	Is this advertised brand trustworthy? (1= Not at all, 5 = very much)
5.	Is the advertised brand reputable? (1= Not at all, 5 = very much)
6.	Does this advertised brand make honest claims? (1= Not at all, 5 = very much)

For each criterion, provide just the answer Do not add any prefix word or symbol ``` or word "json" before output and output should be just like following example Response without any braces { or } or comma. There should not be any comma between the lines

Example for above format. Output should be strictly in below format with no prefixes and just the output: 

"Familiar_with_brand": 3
"consumer_popularity": 4
"brand_perceive_high_quality": 2
"brand_trust_worthiness": 1
"brand_reputability": 5
"brand_honest_claims": 5

"""

#### Other questions

question="""Analyze the commercial video and provide the following information:

Ad time:
1.	What is the total time the brand was mentioned in the ad? (5 seconds)
2.	What is the total time the brand name/logo was displayed in the ad? (10 seconds)

Character presentation:
1.	Does the commercial present a strikingly beautiful character? (No=0, Yes=1)
2.	Does the commercial present a strikingly ugly character? (No=0, Yes=1)


For each criterion, provide just the answer Do not add any prefix word or symbol ``` or word "json" before output and output should be just like following example Response without any braces { or } or comma. There should not be any comma between the lines

Example for above format. Output should be strictly in below format with no prefixes and just the output: 

"brand_total_time_mentioned": 5 seconds
"brand_total_time_displayed": 4 seconds
"beautiful_char_present_ind": 1
"beautiful_char_present_ind": 0

"""
