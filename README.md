# GroupDNA: Your WhatsApp Group Chat, Decoded

GroupDNA reads a WhatsApp chat file and prints a full report about the group. It shows who talks the most, who is the night owl, who goes silent, which words the group uses most, and which personality type each member gets. It is like Spotify Wrapped, but for a friend group.

I made this for The Unlox Academy internship (Week 1 minor project) using only Python basics and NumPy.

## Output

screenshot.png

## What it does

- Reads the chat file line by line and handles system messages, media messages, deleted messages, multi-line messages and empty lines
- Shows the group overview: dates, total messages and messages per person
- Finds the busiest day and the busiest hour
- Builds an activity heatmap using a NumPy matrix (people x hours of the day)
- Finds the top words used by the group
- Measures how fast each person replies and their longest silent streak
- Gives each person a personality archetype, such as The Spammer, The Night Owl or The Ghost
- Prints everything as one clean report

## Dataset

I used hostel_bois.txt, a made-up chat of 6 friends over 60 days with 3,174 messages. It is not a real chat.

## Rules I followed

Used: Python basics, lists, dictionaries, sets, tuples, NumPy, and datetime (only strptime and timedelta).

Not used: pandas, matplotlib, regex, Counter, defaultdict, or any ready-made chat analyzer. The heatmap and charts are made with text characters only.

## How to run

1. Open the notebook in Google Colab
2. Upload hostel_bois.txt using the folder icon on the left
3. Click Runtime > Run all

## Files

- the notebook (.ipynb)
- hostel_bois.txt (dataset)
- screenshot.png (screenshot of the report)
- README.md

## What I learned

Real data is messy, so a good parser matters the most. I also learned how to turn behaviour into numbers, like night-time share and silent days, and how to make sure each archetype goes to only one person.

## Author

Spandana U N
B.E. Artificial Intelligence and Data Science
Navkis College of Engineering, Hassan (VTU)
