# # Making History Speak - AI Avatars for Classroom Adventures : a Design Brief and Curriculum Design Guide by Maria-Teresa Carmier Villalobos


## Introduction
Embarking on the "Making History Speak: AI Avatars for Classroom Adventures" project wasn't just a step into the unknown; it was a leap into a vast chasm that separates the technical from the non-technical, the artist from the coder. My journey began with the George Moses Horton project, an ambitious endeavor to weave the strands of ancient oral traditions into the fabric of modern AI technology. Initially brought on board as an interaction designer, my role soon morphed into something far more complex and daunting.

In the crucible of creation, I became acutely aware of the gulf that lay between the worlds of art and technology. It was a space filled with silos, where non-technical folks like myself often found ourselves underestimated, our potential boxed in by unseen barriers. This wasn't always intentional, but the effect was the same: a reinforcement of a divide that, as a social equity advocate, I was determined to dismantle.

The quest for technical literacy was a steep climb, fraught with moments of self-doubt and the shadow of impostor syndrome looming large. Yet, against expectations, I bridged that gap. The surprise in people's eyes when they realized what I had achieved only highlighted the stereotypes I was battling against.

This journey led me to a pivotal question: How can technology truly serve the greater good? Inspired by this challenge, I envisioned a project that could potentially shrink the chasm of technical literacy, turning technology into a tool for empowerment rather than exclusion. Thus was born the idea for this curriculum guide, a beacon for educators seeking to light up their classrooms with the magic of AI avatars and historical narratives.

This guide is more than just instructions; it's a testament to the journey from feeling like an outsider in the world of tech to harnessing its power for educational innovation. It represents a bridge built not just for myself, but for all educators who dare to dream of a classroom where technology serves as a gateway to history, engagement, and empowerment.

## Objectives
- Familiarize educators with AI tools for creating speaking avatars of historical figures.
- Offer detailed instructions for generating and integrating AI avatars into history lessons.
- Provide strategies for crafting engaging Midjourney prompts for visualizing historical characters.
- Promote interactive and immersive learning experiences within the classroom setting.

## Tools Overview
- **D-ID**: Revitalizes photographs by creating speaking avatars, ideal for interactive historical figure videos.
- **Midjourney**: Generates images from text prompts, perfect for visualizing historical scenes and characters.
- **OpenAI and AWS Polly**: Employs speech-to-text and text-to-speech capabilities, respectively, enabling historical figures to answer student inquiries directly.

## Part 1: Setting Up Accounts and Obtaining Access Keys
### Account Creation
1. Sign up for accounts on **D-ID**, **Midjourney**, **OpenAI**, and **AWS** by visiting their respective websites.
2. Seek educational discounts or programs offered by these platforms for school use.

### Access Keys
- Secure the necessary API keys from each platform. Store these keys safely, and refer to each platform's documentation for steps on integrating these keys into your project.

## Part 2: Creating Your AI Avatar with D-ID
### Objective
Craft a speaking avatar of a historical figure to field student questions and offer insights into their historical context.

### Steps
1. **Select a Historical Figure**: Pick a figure pertinent to your lesson plan.
2. **Gather Resources**: Compile images and biographical texts for your chosen figure.
3. **Generate Speaking Avatar**: Employ D-ID to animate the figure’s image, syncing it with audio from AWS Polly, which narrates the biographical text.

## Part 3: Visualizing Historical Characters with Midjourney
### Objective
Produce visuals of historical characters or scenes to complement lessons, enriching the historical narrative visually.

### Steps
1. **Crafting Prompts**: Develop detailed prompts that describe the historical figure or scene, incorporating physical attributes, attire, and context.
   
   Example: “Create an image of George Moses Horton contemplating in a field, embodying his new status as a Freedman, against a winter backdrop, captured in an oil painting style.”
   
2. **Using Midjourney**: Enter your prompt into Midjourney’s interface to generate the image, tweaking the prompt as necessary for optimal results.

## Part 4: Integrating AI Avatars into Lessons
### Objective
Deploy the crafted AI avatars and images to create interactive lessons, allowing students an opportunity to "meet" historical figures.

### Activity Ideas
- **Q&A Sessions**: Have students prepare questions for the AI avatar, fostering historical dialogue.
- **Visual Discovery**: Employ Midjourney images as catalysts for discussions or creative writing.
- **Role Play**: Integrate avatar videos into role-playing exercises, prompting student responses to the avatars’ narrations.

## Tips for Educators
- **Preview Content**: Review all AI-generated materials for historical accuracy and appropriateness before classroom use.
- **Encourage Critical Thinking**: Urge students to critically evaluate the information presented by AI avatars, contrasting it with other historical sources.
- **Curriculum Integration**: Align activities with curriculum objectives, ensuring they augment and enrich existing lesson plans.

## Creating a Digital Exhibition: History Class Comes to Life
Elevate the learning experience by setting up a digital exhibition titled "History Class Comes to Life," utilizing AR/VR technology. This project, exemplified by the George Moses Horton initiative, aims to celebrate oral storytelling and Black creativity. I lead the interaction of the Avatar and supported the exhibit design
### [GMH Virtual Exhibit](https://gmhvirtual.my.canva.site/gmhexhibitdesign)

### Engaging Students with AR/VR and QR Codes
Implement AR/VR experiences using platforms like Niantic, creating immersive environments that allow students to explore historical contexts firsthand. Enhance interactivity by incorporating QR codes linked to VR experiences, developed on Niantic, offering students a hands-on approach to history.

### Implementing the George Moses Horton Project
This initiative highlights George Moses Horton's legacy, allowing students to engage with his poetry and story through AI avatars. By adding QR codes, educators can further utilize VR technology with Niantic, offering a multi-dimensional exploration of Horton's world.

## Multi-Layered Guide for Creating Speaking Avatars
This section caters to varying levels of technical expertise, from Rhino (expert) to Bunny (beginner), providing a nuanced approach to creating speaking avatars for educational use.

### Incorporating the Python Script
For practical application, here's a simplified Python script ready for customization. This script is designed to be adaptable, allowing educators of

 all technical backgrounds to integrate speaking avatars into their curriculum effectively.

```python
# Simplified Python script for creating speaking avatars
# Note: Replace placeholders with actual API keys and file paths

# Import required libraries
import boto3
import openai
import requests

# Function to read API keys from files
def open_file(filepath):
    with open(filepath, 'r', encoding='utf-8') as infile:
        return infile.read().strip()

# Initialize OpenAI and AWS Polly clients with your API keys
openai.api_key = open_file('path/to/your/openai_api_key.txt')
polly_client = boto3.client('polly', aws_access_key_id=open_file('path/to/your/aws_access_key.txt'), aws_secret_access_key=open_file('path/to/your/aws_secret_key.txt'))

# Example function to generate speech from text and animate an avatar with D-ID
def create_speaking_avatar(text, image_path):
    # Generate speech with AWS Polly
    # [Add AWS Polly speech synthesis code here]
    
    # Animate the historical figure’s image with D-ID
    # [Add D-ID animation code here]

# Use this script to bring George Moses Horton to life in your classroom
create_speaking_avatar("Poetry from George Moses Horton", "path/to/george_moses_horton_image.jpg")
```

### Conclusion
"Making History Speak" empowers educators to merge historical education with cutting-edge AI technology, providing a dynamic and engaging learning environment. Through this guide, teachers can bring historical figures like George Moses Horton into the classroom, offering students a unique and interactive way to explore history.
