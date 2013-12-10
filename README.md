followpie
=========

Instagram loves pie


Follow Pie is a tried and tested Instagram bot which automatically follows and likes users and photos based on certain parameters.

Made by [@mutlu82](https://www.twitter.com/mutlu82 "@mutlu82") and [@oh_moore](https://www.twitter.com/oh_moore "@oh_moore") with the goal of increasing more users for our personal accounts and driving people to view our profile pages which contains a url to our iPhone app

The aim of the bot is to get real people to reciprocate follows and likes.

The bot has several options -
Like
Follow
Set amount of photos to like
Set amount of people to follow
Set the time between each follow/like
Follow and like people who post photos to a certain hashtag, for example #London, will start the bot liking and following those users who have tagged their photo #london
Like and follow users who like photos on the popular page - this sets the bot running on users who have liked a photo on the popular page. The reason for this is because if someone has liked a photo on the popular page it is likely the are a active user and you'll get a quicker reciprocation.

Notes:

When this bot was written there was no limit on how many people you could follow, however it has since changed to 7500

There is also a API request limit of 5000 per second. However there's a limit of photos you can like per hour at around 200-300.

Our testing shows that it takes around 1000 likes to get 10 follows returned. Follow and liking is more powerful and returns better results (people are more inclined to return the favour)

An ideal way to get a better return for the follow like setup is to have the script also unfollow anyone who does not follow you. This would allow the Instagram algorithm to let you have better weighting for your posts.


Technical Stuff.

If you've no idea whta you're doing you can get the bot up and running with the following steps.

1. Download Python http://www.python.org/getit/
2. Run the python IDLE which you get packaged with the python installer for your OS
3. With the IDLE open the script
4. Before running you'll need to get your access token. 
5. To do this you'll need your own web domain and your own developer api access with instagram. http://instagram.com/developer/ Sign up and get an API key that allows you to like and create relationshops. You'll then need to have the authorization url redirect to your authorized web domain. To get your key, replace the appropriate parts of the auth URL you can see in the script like this.

https://api.instagram.com/oauth/authorize/?client_id=1627c123e3fc481791e0d6be16ff57a0&redirect_uri=http://yoururl.com&response_type=token&display=touch&scope=likes+relationships

change the client id to your client id and change the redirect_uri to be the domain you've specified with the auth key, when you get redirected back to your web page you'll be given an auth code in the return url. Copy this code out and add it to the script in the auth_token variable. (e.g. auth_token="authtokenreturnedbyinstagram")

6. Next change tags and the script actions you'd prefer and in the top menu hit Run -> Run Module (F5)



Note* This script is not designed to work in the command line yet as it was meant to be edited visibly by a non command line individual, feel free to change and edit it to run with command line use.

