
## Fake Sushi Website

https://a3-jeemie-jimmy-tran.glitch.me/

Include a very brief summary of your project here. Images are encouraged, along with concise, high-level text. Be sure to include:

This webapp was inspired by the restaurant that I have been working at for 3 years. 
No other type of database would I be more familiar with than a food system. One of the harder challenges
was getting everything to just *work*. learning how to do the post and gets correctly was the biggest challenge
and looking online helped me a lot to implement them, along with a lot of debugging.

Honestly, I've spent way too much time on things that weren't problems, but more of my own stupidity (a lowercase instead of uppercase for example).
Getting passport implemented correctly was extremely difficult and took awhile before it was right.

The way the app works is that you type in your information and choose what fish you'd like, how you'd like to have it,
and of course how much you'd like. After hitting submit, you'll be brought to the All Orders screen which show you orders that's associated with your account.

Keep in mind that if you're not authenticated you'll be unable to go into any page as it'll just redirect you to login everytime. 

The authentication strategy I used is Local, as it is the easiest and was recommended. I already had trouble and wasted a lot of time getting it to work correctly that
I could not afford to use better Auth strategies even though I wish I could. 

I did not use any CSS framework although I did mess around with Pure.CSS for a bit as I really enjoyed the simple layout of my current site. 

Middleware packages actually used:
Passport: Allows authentication
express-session/passport-session: Allows storage of sessions
BCrypt: Hashes passwords so no raw-text is ever stored (I actually knew this one from working in a Maplestory private server, yay!)
Body-parser: Parses json directly into request.body so it's easier to read.
UUID: Generates unique IDs for each session
Views engine that works with EJS templates (I didn't use ejs really but did use the methods a bit, but idk if it really counts as one.)
Filestore: Used to help store the sessions

## Technical Achievements
- **Tech Achievement 1**: Used more than 5 middleware packages
- **Tech Achievement 2**: Multiple pages with tables that load dynamically based on how many orders are stored.
- **Tech Achievement 2.1**: Handles duplicate usernames upon trying to register (It's case sensitive though.. Jimmy != jimmy)
- **Tech Achievement 2.2**: No pages load unless authenticated.. (I know it's just some if statements but that's why it's .1 of an achievement)


