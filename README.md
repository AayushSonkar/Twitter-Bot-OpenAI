# Twitter-Bot-OpenAI

Ever see those Twitter bots that reply to comments automatically? Like this [one](https://twitter.com/explainthisbob/status/1661833808092471299?s=12) or [this one](https://twitter.com/replygpt/status/1661924851626696705?s=12)

Let's create one ourselves. In this notebook we'll just look at the prompting technique I used. In the [full code](https://github.com/gkamradt/twitter-reply-bot) you'll see the other helper code to deploy this app.

Here's how the final app will work

1. A user @mentions your bot, for me it will be @SiliconOracle
2. The script finds that new @mention and then reads the parent tweet it is being mentioned on
3. The script takes that parent tweet and generates a witty response using a language model
4. Respond is posted and tweet is logged

This notebook will focus on #3.

First let's import our packages# Twitter-Bot-OpenAI
