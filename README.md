Project about work with [Beautiful Soup](https://www.crummy.com/software/BeautifulSoup/bs4/doc/).

You can just run `python3 -m http.server` in a directory 
with this file to be able to test 
my little prank in a browser. Just open
http://127.0.0.1:8000/evilcorp.html and you'll see the form yourself. 
___

Python script 'exploit.py' that do several things:

- First, page title changes (in `<title>` tags) to "Evil Corp - Stealing 
  your money every day"
- Second, the name of the user from the page is parse (including the pronoun)
  and injects new tag `<h1>`
  into a `body` of a page, saying `<h1>Mr. Robot, you are hacked!</h1>`, 
  where 'Mr. Robot' is a parsed pronoun
  and name.
- Third, when the 'Send' button is pressed, 
  you see the word "hacked" appearing in an alert window.
- Finally, the link at the bottom of a page now lead to "https://mrrobot.fandom.com/wiki/Fsociety" with 
  an actual name of the company on a page replaced with "Fsociety".