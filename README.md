# SpongebobNovel
A repo to house my markovify AI that trains on individual text files, before combining knowledge and generating a SpongeBob play.

I was inspired to take this route after watching Professor Whalen demonstrate a similar module, also using transcripts from Spongebob. The output was hilarious and I decided that I also wanted some sort of comedic output. After reading through the Markovify api and checking out how a couple different people used it, I decided to see how I could train the AI on various different text documents, but still have a central hivemind. While I used similar text in each of the read-in files, a user could use the works of various different authors and produce a result that combines the styles of each. I had a lot of fun with this project as most of the time the output sentences are barely comprehensible and feel akin to what I believe having a stroke feels like.  

To use this code, the user must create a folder in the working directory named 'training'. Once text files are loaded into this folder, this for loop is modular and can be added infinitely for each file you wish to read in. Just fix the filename3 variable. 

for filename in os.listdir(PATH):

content = open(f'{PATH}{**filename3**}', 'r').readlines()

markov_chain = markovify.Text(content)

chains.append(markov_chain)

____________________________________________________________________________________________________________________________________________________________________

Part: 1

SpongeBob: Well, I'm not the judge of me!

Roderick: Keep your eyes will be carted out in your granny's hand basket.

Mrs. Puff: You don't want to hear your stomach growling.

Patrick: I'm trying to eat my sea chimps his loyal servants.

Plankton: Out of my mind.

Patrick: Well, I've got the best ideas.

SpongeBob: You got a new clock, boy-o.

Squidward: Oh, don't you use this stuff to go find Gary.

Police fish #1: We've got work to do.

Squidward: It's been your constant encouragement that has to do with this?

Patrick: It stopped working so I could tell you something, mister.

SpongeBob: Thanks for the patty toward a sleeping SpongeBob.

Monroe: It's a tiny pipsqueak like you need a new boat.

Plankton: I've never seen another creature that is makes the wood-shaped alarm clock rings
with Patrick making sound effects in the same place for 20 years and you've never noticed
ingredients of the window, a truck with a ball.

