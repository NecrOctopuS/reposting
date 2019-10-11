### Reposting in social networks
The program publishes a post (picture and text) in three social networks:
1. [VKontakte](https://vk.com/)
2. [Telegram](https://telegram.org/)
3. [Facebook](https://www.facebook.com/)


### How to install
To get started, get a token from VK, it can be obtained as follows:

You must follow the link: https://oauth.vk.com/authorize?client_id=`Your_ID_client`&scope=photos,groups,wall,offline&response_type=token
where `Your_ID_ID` is the application ID that can be viewed in the settings of your [application] (https://vk.com/apps?act=manage)

Next, you need to get a token from Telegram, you get it automatically by creating a bot.

You also need a key (access token) with the right to `publish_to_groups` from Facebook, you can get it by following the [link](https://developers.facebook.com/tools/explorer/)
 
The following data must be written to the `.env` file:
```text
ACCESS_VK_TOKEN = "Your key to Vkontakte"
CLIENT_ID_VK = 'Your Vkontakte Application ID'
GROUP_ID_VK = 'ID of your VKontakte group'
ALBUM_ID_VK = 'ID of your Vkontakte album'
TELEGRAM_TOKEN = 'Your Telegram Key'
CHAT_ID_TELEGRAM = 'Your Telegram Channel ID'
GROUP_ID_FB = 'Your Facebook Group ID'
FACEBOOK_TOKEN = 'Your Facebook Key'
```

Python3 should already be installed.
Then use `pip` (or` pip3`, there is a conflict with Python2) to install the dependencies:
```
pip install -r requirements.txt
```


### Objective of the project

The code is written for educational purposes on the online course for web developers [dvmn.org] (https://dvmn.org/).

### How to start

The full path to the image and the full path to the text file with the post text are fed to the input
```
py reposting.py d: \ images \ image.jpg d: \ text \ text.txt
```