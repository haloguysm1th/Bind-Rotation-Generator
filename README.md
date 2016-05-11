# (Dank) Bind Rotation Generator
Clientside web app for silly Source game bind rotations.
 
## Screenshots

![Courtesy of r/copypasta](http://i.imgur.com/7MJri4E.png "navyseal")
![Ingame Team Fortress 2 Chat](http://i.imgur.com/0aGrpFx.png "demoman?")

## Introduction

View the app [here](https://paced.github.io/bind-rotation-generator/).

Why do you need this app? Well, you don't. But it can be a bit of fun. You can use it to turn lengthy, mostly unformatted copypasta or even movie scripts, novels, what have you into a bind rotation. This means you can press a button of choice and it will output a string to chat. Continue pressing it to continue until you get to the end. Then it loops.

I am aware that at least two other apps exist that do the same thing. Despite my own justification that practicing programming is a reason in itself, there's a bit more to it than that. This app is both similar but mostly different to those apps in a variety of ways.

### It's similar in that:

- It runs (almost) completely on the clientside meaning you can simply view it as a plain HTML file on my GitHub. If you want, you can also download it for yourself to use "offline" (you need an internet connection to view the stylesheets.)
- It allows you to name the aliases.
- The method of creating the bind rotation is pretty much the same.

### It's different in that:

- It's styled with Bootstrap. Trivial difference, I know, but it's better than plain HTML.
- No wait commands, helpful for competitive servers.
- The dropdown list for keys to bind is exhaustive, i.e.: every single possible bindable key/mouse trigger is in that list.
- This will split each line to make sure it will fit when you try to use it in server.
- It will detect for empty "say " commands and will not add them to the output.
- You can choose to include a few lines of comments to the config.
- Not sure about the speed of other similar apps, but this can process the entirety of, say, the Bee Movie script in less than a second (depending on your processor). I believe I used a fair few comparisons, though the time difference should be trivial. I tried the same with Les Miserables but it crashed my browser. There's a limit to how much you can mash that spam bind, kids.

### Notes:

- This will not work for excessively long "words" that are longer than 127 letters long. I won't add functionality for something that ridiculous.
- Be careful putting a very, very long string in the generator. The speed/execution of the code is dependent on your machine, not mine, and putting War and Peace in there will probably freeze the page or crash your browser.

## Usage

- Open the [link](https://paced.github.io/bind-rotation-generator/) in your browser or clone the repository to your drive.
- Paste in your long string/text and choose a key.
- *You must apply two alias names in the input boxes. This will allow you to create multiple bind rotations provided you bind different keys. The aliases should not contain any special characters or whitespace.*
- Click "Generate".
- Copy paste the output to either your autoexec.cfg, or create a new file, e.g.: binds.cfg, and put "exec binds.cfg" in your autoexec.
- In game you can press that button to use the rotation.
