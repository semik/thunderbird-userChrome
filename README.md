# Semik's Thunderbird notes

In far a far away history I was using [pine](https://en.wikipedia.org/wiki/Pine_(email_client)) for reading and organizing my emails. I switched to [Thunderbird](https://en.wikipedia.org/wiki/Mozilla_Thunderbird) around it's birthday in 2003, it's quite good. It sucks sometime, but in my option it sucks less than others.

## Visual modifications

You can change a lot of visual aspects of Thunderbird by file userChrome:

```
cd ~/.thunderbird/xyz.default/
git clone https://github.com/semik/thunderbird-userChrome.git chrome
```
To get it working you also set ''toolkit.legacyUserProfileCustomizations.stylesheets'' to ''true'' i Config Editor, it is accesible from General tab of Thunderbird Settings.

### Lines in folder tree and message list

I work with a huge amount of mails on several mail servers. In far away history Thunderbird designers decided to remove lines in folder and message list. Especially in message lists my eyes tends to lost line and assign wrong sender to wrong subject. Different colors for every odd line help me to track line without extra effort. Another aspect is that, big white area attracts attention, I want to put attention to content of email, other parts of email client should not have such dominant color as white is. Solution is style [lines.css](https://github.com/semik/thunderbird-userChrome/blob/master/lines.css), it works for me at least since TB 60. Today I do not remember where I've found solution so I can't credit original author here.

### Icons for folder trees

Thunderbird version 78 came with quite flat design, I like it except default icons for servers and folders, they are quite dominant and all the same to my eyes. One solution is to [color them](https://support.mozilla.org/en-US/kb/new-thunderbird-78#w_customize-the-colors-of-mail-folder-icons), but I do not like this. Other possibility is to use plugin [Phoeity Icons](https://addons.thunderbird.net/en-US/thunderbird/addon/phoenity-icons/?src=dp-dl-othersby) but that is too much colorful to me. I was used to those original icons, solution is in [icons.css](https://github.com/semik/thunderbird-userChrome/blob/master/icons.css) taken from  [post in MozillaZine](http://forums.mozillazine.org/viewtopic.php?f=30&t=3064381&p=14873377#).

### Open & closed folder lists

Open & closed folder lists have quite big arrows which are looking nice with TB78 flat icons but not with the old one. See [twisty.css](https://github.com/semik/thunderbird-userChrome/blob/master/twisty.css) for solution. I'm glad I learned new word 'twisty' which is used for this type of widget.

![My TB](https://github.com/semik/thunderbird-userChrome/blob/master/example.thunderbird.png)

### Blue color for new message and folder with new message

Thunderbird 78 started using light green for account name in folder panel which have quite low contrast for me. I've discovered how to change color of new message in message panel, color of folder in folder tree but I'm still [struggling with color of account](https://support.mozilla.org/cs/questions/1319249). See [colors.css](colors.css).


## Plugins
