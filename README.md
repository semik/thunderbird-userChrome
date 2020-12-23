# Semik's Thunderbird notes

In far a faraway history I was using [pine](https://en.wikipedia.org/wiki/Pine_(email_client)) for reading and organizing my emails. I switched to [Thunderbird](https://en.wikipedia.org/wiki/Mozilla_Thunderbird) around its birthday in 2003, it's quite good. It sucks sometimes, but in my option, it sucks less than others.

## Visual modifications

You can change a lot of visual aspects of Thunderbird by file userChrome:

```
cd ~/.thunderbird/xyz.default/
git clone https://github.com/semik/thunderbird-userChrome.git chrome

```

To get it working you also set ''toolkit.legacyUserProfileCustomizations.stylesheets'' to ''true'' i Config Editor, it is accessible from the General tab of Thunderbird Settings.

### Lines in the folder tree and message list

I work with a huge amount of mails on several mail servers. In faraway history, Thunderbird designers decided to remove lines in the folder and message list. Especially in message lists my eyes tend to lost line and assign a wrong sender to a subject. Different colors for every odd line help me to track line without extra effort. Another aspect is that the big white area attracts attention, I want to put attention to the content of an email, other parts of the email client should not have such dominant color as white is. The solution is style [lines.css](https://github.com/semik/thunderbird-userChrome/blob/master/lines.css), it works for me at least since TB 60. Today I do not remember where I've found the solution so I can't credit the original author here.

### Icons for folder trees

Thunderbird version 78 came with quite a flat design, I like it except for default icons for servers and folders, they are quite dominant and all the same to my eyes. One solution is to [color them](https://support.mozilla.org/en-US/kb/new-thunderbird-78#w_customize-the-colors-of-mail-folder-icons), but I do not like this. Another possibility is to use a plugin [Phoeity Icons](https://addons.thunderbird.net/en-US/thunderbird/addon/phoenity-icons/?src=dp-dl-othersby) but that is too much color for me. I was used to those original icons, solution is in [icons.css](https://github.com/semik/thunderbird-userChrome/blob/master/icons.css) taken from  [post in MozillaZine](http://forums.mozillazine.org/viewtopic.php?f=30&t=3064381&p=14873377#).

### Open & closed folder lists

Open & closed folder lists have quite big arrows which are looking nice with TB78 flat icons but not with the old ones. See [twisty.css](https://github.com/semik/thunderbird-userChrome/blob/master/twisty.css) for solution. I'm glad I learned the new word 'twisty' which is used for this type of widget.

![My TB](https://github.com/semik/thunderbird-userChrome/blob/master/example.thunderbird.png)

### Blue color for new message and folder with a new message

Thunderbird 78 started using light green for account name in folder panel which has quite low contrast for me. I've discovered how to change the color of a new message in the message panel, the color of a folder in the folder tree but I'm still [struggling with the color of account](https://support.mozilla.org/cs/questions/1319249). See [colors.css](colors.css).

## Plugins

### Nostalgy++

[Manage emails / Nostalgy++](https://addons.thunderbird.net/en-US/thunderbird/addon/nostalgy_ng/) essential plugin! I can't use TB without it. I'm using it for moving email into a folder only by the keyboard.

### Simple Mail Redirection

[Simple Mail Redirection](https://addons.thunderbird.net/en-US/thunderbird/addon/simple-mail-redirection/) Bunce from Pine - essential if you are using RT or a similar ticketing system but users keep sending emails directly to your personal email.

### DKIM Verifier

[DKIM Verifier](https://addons.thunderbird.net/en-US/thunderbird/addon/dkim-verifier/) a tool used for verification of automatic signatures from domains.