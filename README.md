Bleep, bloop, imma bot!

Here are some important things you will want to know about the me:

🤖   Expected Behaviour: 
- It will ping a pending reviewer if they have not reviewed or commented on the PR in x days since the last update or the last time the bot pinged them. (default x = 3)
- It will ping the author of the PR if they have not addressed a review on a PR after x days since last review or the last time the bot pinged them. It will also ping them to remind them to re-request review if needed.  (default x = 3)


🤖  Controls 
To control the bot, you need to add a comment on the PR starting with !lightninglabs-deploy followed by the command. There are 2 control types: mute/unmute & cadence. Only the latest comment for each control type will be used. This also means you dont need to keep adding new control comments, just edit the latest comment for that control type. 
- !lightninglabs-deploy mute will mute the bot on the PR completely. 
- !lightninglabs-deploy mute 72h30m will mute the bot for the given duration.
- !lightninglabs-deploy mute 2022-Feb-02 will mute the bot until the given date (must be in this format!).
- !lightninglabs-deploy mute #4 will mute the bot until the given PR of the same repo has been merged.
- !lightninglabs-deploy unmute will unmute the bot (or just delete the comment that was muting it)
- !lightninglabs-deploy cadence 60h change the cadence of the bot from the default of 3 days to the given duration.
- it will automute if the PR is in Draft mode

🤖 For now, the lbot will continue to post in #code-review. Maybe we can eventually turn that off if the above works well enough. 

🤖 Apologies in advance for the many notifications that many of you will get when this bot first kicks off 😅 Just maybe take some time to go mute / set cadences / ping dependencies etc to optimise for high signal pings

🤖 if the behaviour of the bot seems to differ from what is expected, please open an issue in the lbot repo and assign me & link the PR and bot-action in question
