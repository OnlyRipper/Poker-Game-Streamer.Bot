## This is my first attempt on making something like this, so there might be LOTS of BUGS for now, I will try to fix any problems asap!
## Many thanks to the original files and [streamerbot.com ](https://streamer.bot/) which I used.

Game adjusted to work in Streamer.bot with 2 players playing against each others. (Twitch only).

　🔘 Web socket server required with default port 8080.

　🔘 Download the .zip file - Extract the folder anywhere in your PC - Add a browser source in OBS (check Local file box) locate and add the    
　　　　　　　　　　　　　intex.html file, uncheck Shutdown and Refresh boxes if checked.

　🔘 You must be using a Twitch Bot inside Streamer.Bot ( If you don't have one, just make an account and connect it).

　🔘 I'm using Twitch Whispers System to send the cards values to the players, there are limitations and your chatbot must have a verified
　　　 phone number you can read more here: https://docs.streamer.bot/api/triggers/twitch/chat/bot-whispers#notes 
　　　　　*Also, users must have whispers enabled or to message the bot first in order to receive them.

　🔘 It works with Currency Core extension ( https://extensions.streamer.bot/docs?topic=49 ) just enable the subAction.

　🔘 Download the .txt file and copy all the text inside - Go to Streamer.Bot - Imports Tab - Add the text to the Import Field.
 　　　[Copy ME.txt](https://github.com/user-attachments/files/16776644/Copy.ME.txt)

　🔘 In the Sub-Actions check all the comments and replace the fields with yours
  
　![SB subActions](https://github.com/user-attachments/assets/eb5fb5ed-6dd5-4c23-b8ab-36235ac0d770)

　🔘 Images:
　　![image](https://github.com/user-attachments/assets/9936b17a-35c1-4ac2-9403-758a25713a82)

![image](https://github.com/user-attachments/assets/dda09d06-26e5-4dad-8340-e4273c906493)
 
　🔘Commands: ◻️ !pokerstart (Starts a game for anyone to join with default bet) or add any amount after the command to set the pot.
‎　　　　　　　　◻️ !pokerjoin (Join a game if available). 
　　　　　　　　◻️ !pokerend (Force end a game with no winners).
　　　　　　　　◻️ !poker (This is the main command to trigger actions, add the action you want to take after the command, ex: !poker check
　　　　　　　　　　　　◻️ check (skips your turn and waits for the opponent action).
　　　　　　　　　　　　◻️ raise (type your chosen amount of raise after, ex: !poker raise 100
　　　　　　　　　　　　◻️ reraise (only works if opponent already raised, same as raise add the amount after, ex: !poker reraise 100
　　　　　　　　　　　　◻️ allin (this puts all your points on the pot, if you have more than your opponent, it automatically picks their max 
　　　　　　　　　　　　　　　points and sets the bet to that).   
　　　　　　　　　　　　◻️ call (calls any raise, reraise or allin).
　　　　　　　　　　　　◻️ fold (give up and quit the game).        
  
　🔘 The browser source has a small delay between showing the cards, a message in chat will be sent short time after the cards are shown 
　　　on the screen to compensate for the Twitch delay.
