# SpongebobNovel
A repo to house my markovify AI that trains on individual text files, before combining knowledge and generating a SpongeBob play.

I was inspired to take this route after watching Professor Whalen demonstrate a similar module, also using transcripts from Spongebob. The output was hilarious and I decided that I also wanted some sort of comedic output. After reading through the Markovify api and checking out how a couple different people used it, I decided to see how I could train the AI on various different text documents, but still have a central hivemind. While I used similar text in each of the read-in files, a user could use the works of various different authors and produce a result that combines the styles of each. I had a lot of fun with this project as most of the time the output sentences are barely comprehensible and feel akin to what I believe having a stroke feels like.  

To use this code, the user must create a folder in the working directory named 'training'. Once text files are loaded into this folder, this for loop is modular and can be added infinitely for each file you wish to read in. Just fix the filename3 variable. 

for filename in os.listdir(PATH):
  content = open(f'{PATH}{**filename3**}', 'r').readlines()
  markov_chain = markovify.Text(content)
  chains.append(markov_chain)
