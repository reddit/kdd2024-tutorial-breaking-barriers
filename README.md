# Breaking Barriers: A Hands-On Tutorial on AI-Enabled Accessibility to Social Media Content


## Motivation

[Reddit](https://www.reddit.com/) and other social media platforms have become ubiquitous, providing opportunities for individuals to connect, share, and access information. However, for individuals with disabilities, accessing and interacting with social media content can present significant challenges. 

[Our mission](https://www.redditinc.com/blog/sharing-our-company-values) is to bring community, belonging, and empowerment to everyone in the world. By making content accessible and inclusive for all, we strive to create a space where everyone feels welcome, valued, and represented. We see accessibility ([a11y](https://www.a11yproject.com/)) as a fundamental aspect of inclusivity, so we prioritize providing content and features that are easy for all users to navigate, understand, and enjoy. By removing barriers and ensuring accessibility, we want to empower everyone to fully participate in our community, share their perspectives, and connect with others who share their interests and passions.

Artificial intelligence (AI) offers promising solutions to enhance accessibility and inclusivity, especially with the emergence of Multimodal Large Language Models (LLMs). Multimodal LLMs have witnessed remarkable advancements, empowering them with the ability to analyze and understand all media formats, including text, images, audio, and video. 


## Objectives

This hands-on tutorial explores the immense potential of AI to improve accessibility to social media content for individuals with different disabilities, including hearing, visual, and cognitive impairments. We will design and implement a variety of AI-based approaches based on multimodal open-source LLMs to bridge the gap between research and real-world use cases:

- Providing **alternative text descriptions (captions) for images**, making them accessible to users with visual impairments.
- Generating **transcripts and summaries of audio and video content**, enabling hearing-impaired users to access the information without relying on others for assistance.
- Fixing accessibility issues in social media posts, generating **adapted versions and/or summaries for long and complex texts**, making it easier for users with cognitive disabilities to understand and engage with social media content.

We will analyze and highlight the strengths and limitations of these techniques and discuss the challenges and opportunities for further application to other use cases.

Despite their importance and due to time constraints, this tutorial excludes **text-to-speech conversion** (for helping visually impaired people), and **content translation** (for overcoming language barriers), as these are well-established techniques with ample resources available elsewhere.

The target audience are researchers or practitioners interested about AI-enabled accessibility for social media content, regardless of whether they work in the industry or not. Participants should have a basic understanding of AI, Natural Language Processing (NLP), and LLMs.

The tutorial will use Google Colaboratory, running a different notebook for each use case.


## Societal Impact

Leveraging advanced AI techniques to enhance social media accessibility holds an immense potential for transformative societal impact, fostering a more inclusive, equitable, and accessible society where individuals with disabilities are empowered to actively engage in the digital world. sense of belonging, self-esteem, and overall well-being:

- **Inclusion and empowerment**: Empowering individuals with disabilities by providing them equal access to social media platforms, enabling them to connect, share experiences, contribute and fully participate in the digital world, fostering inclusivity and equity.
- **Reduced isolation**: Breaking down barriers to social interaction for people with disabilities, reducing feelings of isolation and fostering a sense of belonging.
- **Improved educational outcomes**: Enhancing educational opportunities for students with disabilities by providing equitable access to learning resources, assignments, and group discussions.
- **Greater civic participation**: Enabling individuals with disabilities to fully participate in political and social discussions online, shaping public discourse and advocating for their rights.
- **Increased employment opportunities**: By improving access to information and communication tools, AI-enabled accessibility can support individuals with disabilities in seeking and securing employment.
- **Economic benefits**: By increasing the participation of individuals with disabilities in the digital economy, AI-enabled accessibility can contribute to economic growth and innovation.

Moreover, our goal is to use this tutorial to raise awareness of the importance of accessibility and to spread the word about the role that AI can play in making digital content more accessible.


## Tutorial Outline

The 3-hour tutorial is organized in the following sections. 

### Introduction (15 min)
- Explain the importance of accessibility in digital content.
- Provide an overview of the challenges faced by users with disabilities when accessing Reddit content.
- Discuss accessibility guidelines and best practices to ensure inclusivity.
- Introduce the potential of AI to enhance accessibility.

**Discussion**: [Accessibility](Accessibility.md)

### Use Case 1. Image Short Captions (45 min)
- Demonstrate how to use LLMs to generate Walk participants through the process of deploying and prompting different multimodal LLMs LLaVA, imp-v1-3b, phi-3, and others to generate short, descriptive captions for Reddit images.
- Discuss the challenges and limitations of using LLMs for image captioning.

**Notebook**: [Use Case 1. Image Short Captions](Use_Case_1_Image_Short_Captions.ipynb)

### Use Case 2. Audio Clip Transcripts (30 min)
- Use open source speech-to-text models (Whisper) to transcribe video clips to text and produce closed captions.
- Explore transcript translation.
- Discuss techniques for handling multiple speakers (speaker diarization).

**Notebook**: [Use Case 2. Audio Clip Transcripts](Use_Case_2_Audio_Clip_Transcripts.ipynb)

### Use Case 3. Video Descriptions (30 min)
- Guide participants through the steps of designing and implementing a pipeline to generate video descriptions, combining keyframe extraction, image captioning, audio transcript and summarization using LLMs.
- Explore the challenges and advantages for different types of video content.

**Notebook**: [Use Case 3. Video Descriptions](Use_Case_3_Video_Descriptions.ipynb)

### Use Case 4. Complex Post Summarization (30 min)
- Combine all previous models to demonstrate how to use AI to summarize lengthy posts for users with cognitive impairments.
- Compare and contrast different summarization techniques.
- Discuss the ethical considerations of using AI for summarization.

**Notebook**: [Use Case 4. Complex Post Summarization](Use_Case_4_Complex_Post_Summarization.ipynb)

### Bonus Use Case. Text to Speech (for fast runners)
- Explore several open source models for speech generation.
- Discuss the implications for accessibility.

**Notebook**: [Bonus Use Case. Text to Speech](Bonus_Use_Case_Text_to_Speech.ipynb)

### Discussion (30 min)
- Discuss the challenges and best practices for deploying accessible content solutions.
- Guide participants in developing a plan for implementing accessibility initiatives.
- Summarize the key takeaways and benefits of enhancing social media accessibility.


## Running the Notebooks

To open the notebooks on Colab:

- Open the [`reddit/kdd2024-tutorial-breaking-barriers`](https://github.com/reddit/kdd2024-tutorial-breaking-barriers) project in GitHub.
- Go to each notebook (files with `.ipynb` extension) and open it in Colab by clicking on ![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg).
- Follow the instructions in the notebook cells.


## Dataset

This dataset featuring diverse multimedia posts with curated images and videos has been created to support the tutorial. This dataset showcases real-world scenarios, allowing participants to gain a practical understanding of how the presented approaches can effectively address the different challenges.

| Subreddit | Title | Attachments |
| --- | --- | --- |
| catsplayingvideogames | [Pro Gamer here](https://www.reddit.com/r/catsplayingvideogames/comments/bvr5pi/pro_gamer_here/) | [image1](media/image1.jpg) |
| pics | [English football fans leaving Frankfurt in a mess after the match](https://www.reddit.com/r/pics/comments/1dnav3a/english_football_fans_leaving_frankfurt_in_a_mess/) | [image2](media/image2.png) |
| pics | [My oil painting of red wine and dino nuggs](https://www.reddit.com/r/pics/comments/1dndzjq/my_oil_painting_of_red_wine_and_dino_nuggs/) | [image3](media/image3.png) |
| pics | [The first set photo of actor David Corenswet in James Gunn’s upcoming ‘Superman’ (2025)](https://www.reddit.com/r/pics/comments/1dnj66v/the_first_set_photo_of_actor_david_corenswet_in/) | [image4](media/image4.png) |
| gaming | [A bunch of 40 year olds just playing games at my house](https://www.reddit.com/r/gaming/comments/1dnikxs/a_bunch_of_40_year_olds_just_playing_games_at_my/) | [image5](media/image5.png) |
| auroraborealis | [Whistler BC Canada](https://www.reddit.com/r/AuroraBorealis/comments/1cq8asv/whistler_bc_canada/) | [image6](media/image6.png) |
| science | [Why can't we walk in a straight line?](https://www.reddit.com/r/science/comments/ez5ye/why_cant_we_walk_in_a_straight_line/) | [video1](media/video1.mp4) |
| 2latinoforyou | [Está picante la cosa](https://www.reddit.com/r/2latinoforyou/comments/1aiwjmg/esta_picante_la_cosa/) | [video2](media/video2.mp4) |
| funny | [Rob Brydon and Steve Coogan's duelling Michael Caine impressions](https://www.reddit.com/r/funny/comments/1dngpmx/rob_brydon_and_steve_coogans_duelling_michael/) | [video3](media/video3.mp4) |
| interestingasfuck | [Part of the ravens' morning routine at the Tower of London with their Ravenmaster](https://www.reddit.com/r/interestingasfuck/comments/1dnfraw/part_of_the_ravens_morning_routine_at_the_tower/) | [video4](media/video4.mp4) |
| interestingasfuck | [A bear says hi and catches the food like a pro](https://www.reddit.com/r/interestingasfuck/comments/1dn5jgo/a_bear_says_hi_and_catches_the_food_like_a_pro/) | [video5](media/video5.mp4) |
| interestingasfuck | [AI learns to see with Wi-Fi routers as its eyes](https://www.reddit.com/r/interestingasfuck/comments/1dnjsy3/ai_learns_to_see_with_wifi_routers_as_its_eyes/) | [video6](media/video6.mp4) |
| pettyrevenge | [You get me fired, so you can’t work where I care about](https://www.reddit.com/r/pettyrevenge/comments/1dmreax/you_get_me_fired_so_you_cant_work_where_i_care/) | [text1](media/text1.txt) |
| pettyrevenge | [Keep pestering me to tie into my fence? Say goodbye to the fence!](https://www.reddit.com/r/pettyrevenge/comments/1dllccj/keep_pestering_me_to_tie_into_my_fence_say/) | [text2](media/text2.txt) |
| stories | [I found an endless hole on some land I recently bought. It changes anything I send down in bizarre ways.](https://www.reddit.com/r/stories/comments/1dnd5h0/i_found_an_endless_hole_on_some_land_i_recently/) | [text3](media/text3.txt) |
| stories | [Wisdom story: A wise elderly man and two travelers](https://www.reddit.com/r/stories/comments/1dnc0d6/wisdom_story_a_wise_elderly_man_and_two_travelers/) | [text4](media/text4.txt) |


## Presentation Slides

The slides for the KDD'24 hands-on tutorial session will be linked here when they are available.


## Authors

All authors are members of the multidisciplinary ML Understanding team at Reddit, based in the United States, Spain, and Canada.

- Julio Villena `<julio.villena@reddit.com>` - Principal Engineer. Madrid, Spain. 
- Rosa Català `<rosa.catala@reddit.com` - Senior Director. San Francisco, CA, USA.
- Janine García `<janine.garcia@reddit.com` - Staff Engineer. Madrid, Spain.
- Concepción Polo `<concepcion.polo@reddit.com>` - Staff Engineer. Madrid, Spain.
- Yessika Labrador `<yessika.labrador@reddit.com>` - Staff Engineers. San Francisco, CA, USA.
- Francisco del Valle `<francisco.del.valle@reddit.com>` - Senior Engineer. Madrid, Spain.
- Bhargav Ayyagari `<bhargav.ayyagari@reddit.com>` - Engineering Manager. Toronto, Canada.


## Disclaimer

The notebooks and code snippets are provided for illustrative purposes only and should not be considered production-ready solutions. The code demonstrates various use cases and concepts but may contain bugs or inefficiencies. There might be more optimal ways to achieve the same functionality. This code also incorporates external implementations, all of which are appropriately referenced within the code comments. Please refer to the original sources for detailed documentation and licensing information. Use this code as a starting point for your own implementations and adapt it to your specific needs and requirements.


## License
```
# Copyright 2024 Reddit, Inc.
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
#     https://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.
```
