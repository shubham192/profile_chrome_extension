<h2 align= "center"><b> Profile Chrome Extension </b></h2>

Are you someone who is active on multiple social media platforms📱?

<p align= "center"><img src="https://media.giphy.com/media/LWFXXqaSEmO7twXDxP/giphy.gif"></p>

Well if the answer is Yes💃,your Bookmarks Bar must be cluttered with them?

<p align= "center"><img src="https://media.giphy.com/media/3ELDuBKag7o8E/giphy.gif"></p>

Want to clean it up a bit?🧹 But what about those one-click solutions you had? Can you preserve them?

<p align= "center"><img src="https://media.giphy.com/media/H6JdkRnhXQaImiCYp2/giphy.gif"></p>

Definitely you can with your custom chrome extension 💻. 

<p align= "center"><img src="https://media.giphy.com/media/nFjDu1LjEADh6/giphy.gif"></p>

Wondering who is gonna build that classy thing for you?🤔🤔 Look no further. You are covered!

<p align= "center"><img src="https://media.giphy.com/media/12FfNKPlSR5k2c/giphy.gif"></p>

<h2 align= "center"><b> Lets see what we have here 👀: </b></h2>

<p align= "center"><img src="https://github.com/smaranjitghose/profile_chrome_extension/blob/master/assets/snapshot.png"></p>

<h2 align= "center"><b> Want it for yourself? Here you go </b></h2>

<p align= "center"><img src="https://media.giphy.com/media/KamhkkcTtvOJ0FCjnB/giphy.gif"></p>

- Clone this repository ⏬
- Move inside 👉 the repo 
    - Open the Terminal 👩‍💻
    - and type ```cd profile_chrome_extension```

- Lets start with the assets you need to modify:
    - You need an icon (mostly your name's initial's in some fancy font) 
    - Resize it to 128x128 and 19x19 px respectively(you can experiment with other sizes too, these are what worked for me). You can use [ResizeImage](https://resizeimage.net/) for this
    - Save them as ```your_name_profile_icon_small.png``` and ```your_name_profile_icon_big.png``` inside the ```assets``` folder(YOu can also use other extensions like .jpg)
    - Now take your favorite profile picture and [resize]((https://resizeimage.net/)) it to 50X50 px (Again, this worked for me. You are welcome to experiment with other sizes) 
    - Save it as ```your_name_picture.png``` inside the ```assets``` folder
- Cool!, you lets have a look at the most crucial file of our Chrome Extension: ```manifest_json```
- Open it in your favourite IDE. (I always prefer [VS Code](https://code.visualstudio.com/) )
- By default, it looks like this:

```js
{
  "manifest_version": 2,
  "name": "My Profile Hub",
  "description": "All my profiles under the same roof",
  "version": "0.0.2",
  "icons": { "128": "assets/smaranjit_ghose_profile_icon_big.png" },
  "browser_action": {
    "default_icon": "smaranjit_ghose_profile_icon_small.png",
    "default_popup": "popup.html"
  },
  "permissions": ["activeTab"]
}
```
<p align= "center"><img src="https://media.giphy.com/media/SqmkZ5IdwzTP2/giphy.gif"></p>

- Don't worry! We are in this together. Let's do this one step at a time.
    - First Update the name you want to give to your chrome extension
     ```js
    "name": "Your_Profile_Extension_Name",
    ```
    - Now,give a small description about it
    ```js
      "description": "All my profiles under the same roof",
    ```
    - (Optional)Decide the version you want to start with. I prefer starting with 0.0.1
    ```js
      "version": "version_number",
    ```
    - Now, Lets give it your icon
    ```js
      "icons": { "128": "assets/your_name_profile_icon_big.png" },
    ```
    - And finally the default icon(the 19x19 one)
    ```js
    "default_icon": "assets/your_name_profile_icon_small.png",
    ```
- Save ⚓ the changes to the File
- That was easy right?. Now, lets see the basic web dev mantra behind our extension

<p align= "center"><img src="https://media.giphy.com/media/3oz8xRF0v9WMAUVLNK/giphy.gif"></p>

- Open the ```popup.html``` in your favourite IDE (Again,I prefer [VS Code](https://code.visualstudio.com/) )
  - Change the title:
  ```html
     <title>Your_Profile_Extension_Name</title>
  ```
  - (Optional)If you have some specific font in mind. You can change it here: [Here we are using [Google Fonts](https://fonts.google.com/)]
    ```html
    <link
      href="https://fonts.googleapis.com/css?family=your+font+name"
      .
      .
    />
    ```
  - Now scroll down to the ```<body>``` tag
  - Upate your profile picture and name of your chrome extension (A small Tip:Don't make it too long)
  ```html
     <img class="logo-icon" src="assets/your_profile_icon.png" />Your_Chrome_Extension_Name
  ```
  - Now update with a one-line description or perhaps a note for yourself
  ```html
     <p>All my profiles under the same roof</p>
  ```
  - Finally, update your social media profile links:(Delete the given links if you don't use any of the social media platforms mentioned)
  ```html
    <a href="http://your_website_link/" target="_blank">
    <i class="fa fa-laptop" style="color:#122cc4 "></i>
    </a>
  ```
  ```html
    <a href="https://www.linkedin.com/in/your_linkedin_username" target="_blank">
    <i class="fa fa-linkedin" style="#3c797b "></i>
    </a>
  ```
  ```html
    <a href="https://github.com/your_github_username" target="_blank">
    <i class="fa fa-github" style="color:#b5651d "></i>
    </a>
  ```
  ```html
    <a href="https://medium.com/@your_medium_username" target="_blank">
    <i class="fa fa-medium" style="color:#000000"></i>
    </a>
  ```
  ```html
     <a href="https://twitter.com/your_twitter_username" target="_blank">
     <i class="fa fa-twitter" style="color:#0ed1eb "></i>
     </a>
   ```
- Save ⚓ the changes to the File 
- Damn! That was a lot of changes. Now let's use our chrome extension.

<p align= "center"><img src="https://media.giphy.com/media/WgRqTUQbqULJEq9swo/giphy.gif"></p>

   - Open Google Chrome
   - In the Search Bar, type ```chrome://extensions```
   - Enable Developer Mode option (If not already done)
   - Click on ```Load Unpacked```
   - Navigate to the ```profile_chrome_extension``` directory and select it

- Baam!💣 you just made your own Chrome Extension💻 for handling your social media profiles

<p align= "center"><img src="https://media.giphy.com/media/3o7btNa0RUYa5E7iiQ/giphy.gif"></p>

 <h2 align= "center"><b>Want to take this a step further? And share it with the world!</b></h2> 

<p align= "center"><img src="https://media.giphy.com/media/l0Exdm9UbTHAFcJi0/giphy.gif"></p>

- Compress all the content of the ```profile_chrome_extension``` into a .zip file 📦
- Go to [Chrome Webstore](https://developer.chrome.com/webstore/publish). Please carefully read the instructons
- Make sure you have a snapshot📸  of your Chrome extension working in 1280x800 px saved
- Now click on the [Chrome Developer Dashboard](https://chrome.google.com/webstore/developer/dashboard)
- Log in with your Google Account.
- Accept the terms
- Pay the one-time registration fees💰 . (The last time I checked it was around 5$)
- Click on Add New
- Locate your compressed chrome extension 📦in your system and select it
- Select your snapshot 📷
- Click Publish

Boom!💥  You are a Google Chrome Extension Developer now and just got your first extension published (FYI:Give it some hours to be done)

<p align= "center"><img src="https://media.giphy.com/media/VACYDIiciYDtu/giphy.gif"></p>

# Always grateful 🙏 to Professor [Daniel Shiffman](https://www.youtube.com/channel/UCvjgXvBlbQiydffZU7m1_aw) for his tutorials and walkthroughs

<p align= "center"><img src="https://media.giphy.com/media/AeWoyE3ZT90YM/giphy.gif"></p>

 <h2 align= "center"><b>  License 📜</b></h2>

[MIT License](https://github.com/smaranjitghose/profile_chrome_extension/blob/master/LICENSE)

# **Crafted with ❤ by Smaranjit Ghose**

[![built with love](https://forthebadge.com/images/badges/built-with-love.svg)](https://github.com/smaranjitghose) [![smile please](https://forthebadge.com/images/badges/makes-people-smile.svg)](https://github.com/smaranjitghose) 
***
