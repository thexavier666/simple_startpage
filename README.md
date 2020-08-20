# Startpage

![Peek](sample.gif)

This is my attempt at creating a simple, lightweight and javascript-free startpage.

I deliberately didn't put a custom search bar because the default search bar suits me more.

## Installation

1. Clone/download repository in anyplace.
I placed it on my Raspberry Pi, thus the startpage can be accessed by multiple devices.
2. Host the directory using any http server.
I use `python3`'s built-in http server like this

		python3 -m http.server <port> 

3. Open your browser of choice.
I use Firefox.
4. Set homepage as `http://<server IP>:<port>` in **Settings**

### Set the startpage as the newtab

Firefox does not allow custom newtab by default.
You need an extension for this to work.

1. Download [New Tab Override][1]
2. Open the extension
3. Set options as **custom URL**
4. Set URL as `http://<server IP>:<port>` like before

## Cutomization

The color scheme can be easily customized by editing `style.css` file.
I've set all the color codes at the top of the file so that you don't have to hunt them in the file.

If you are going to use more than 3 rows of links in the startpage, consider adjusting

	.content height

[Image source][2]

[1]: https://addons.mozilla.org/en-US/firefox/addon/new-tab-override/
[2]: https://1041uuu.tumblr.com/
