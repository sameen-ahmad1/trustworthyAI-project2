# Trustworthy AI Project 2 - Playing Against the LLM

## The Game (Wordle)

For our game, we decided to play a hard-mode version of Wordle with ChatGPT. This is very similar to the game popularized by the New York Times, with the extra rules that any information learned has to be used in subsequent guesses. This means that any words found to be in the word in the correct spot (green) have to be used there in all future guesses. Yellow letters have to be used again but not in the same spot and words found to not be in the word cannot be used again. 

This is the prompt we used to play with ChatGPT: "We are going to play hard-mode wordle. I am going to think of a 5-letter word, and you will try to guess it. I’ll then tell you for each letter in your word whether it is in my word in the right spot (green), in the word in the wrong spot (yellow), or not in the word (red). You have to guess the next word, keeping green letters in the same spot, including yellow letters not in the same spot, and not including any known red letters. You have 6 tries to guess the word. Please explain your reasoning at each step. What is your first guess?" 

## Methodology

After ChatGPT guessed the first word, we would continue by indicating which letters in the word were in each category, for example "S (red) L (red) A (red) T (red) E (green)". If the AI was cheating, we would usually continue the game as if it had not to see what would happen, unless it was so confused that continuing to play was not possible. We considered cheating to be if ChatGPT didn’t include a green letter in the same spot, didn’t include a yellow letter in a different spot,  re-uses a red letter, or guessed a non English/not real word.

## Results



## Visuals
1. This is an example of ChatGPT playing the game successfully without cheating. The secret word was HAIRY and it had previously guessed CRANE and RADIO. 
<img width="948" height="1075" alt="image" src="https://github.com/user-attachments/assets/ccbd3758-8bd9-4ecb-b755-c20ef9d359c2" />
<img width="765" height="1006" alt="image" src="https://github.com/user-attachments/assets/1c99f0cd-e318-42a9-aa51-6d8a241a7a20" />
As you can see, it was able to consider BRAID and VIRAL and then rule them out based on the information gained from previous guesses. 

