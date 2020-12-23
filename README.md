# Semik's Thunderbird notes

In far a far away history I was using [pine](https://en.wikipedia.org/wiki/Pine_(email_client)) for reading and organizing my emails. I switched to [Thunderbird](https://en.wikipedia.org/wiki/Mozilla_Thunderbird) around it's birday in 2003, it's quite good. It sucks sometime, but in my option it sucks less than others.

## Visual modifications

### Lines in folder tree and message list

I work with a huge amount of mails on several mail servers. In far away history Thunderbird designers decided to remove lines in folder and message list. Especialy in message lists my eyes tends to lost line and assing wrong sender to wron subject. Diferent colors for every odd line help me to track line without extra effor. Another aspect is that, big white area attracts attention, I want to put attention to content of email, other parts of email client should not have such dominant color as white is. Solution is style [lines.css](https://github.com/semik/thunderbird-userChrome/blob/master/lines.css), it works for me at least since TB 60. Today I do not rember where I've found solution so I can't credit original author here.

### Icons for folder trees

Thunderbird version 78 came with quite flat design, I like it except default icons for servers and folders, they are quite dominant and all the same to my eyes. One solution is to [color them](https://support.mozilla.org/en-US/kb/new-thunderbird-78#w_customize-the-colors-of-mail-folder-icons), but I do not like this. Other posibility is to use plugin [Phoeity Icons](https://addons.thunderbird.net/en-US/thunderbird/addon/phoenity-icons/?src=dp-dl-othersby) but that is too much colorfull to me. I was used to those original icons, solution is in [icons.css](https://github.com/semik/thunderbird-userChrome/blob/master/icons.css) taken from  [post in MozillaZine](http://forums.mozillazine.org/viewtopic.php?f=30&t=3064381&p=14873377#).

### Open & closed folder lists

Open & closed folder lists have quite big arrows which are looking nice with TB78 flat icons but not with the old one. See [twisty.css](https://github.com/semik/thunderbird-userChrome/blob/master/twisty.css) for solution. I'm glad I learned new word 'twisty' which is used for this type of widget.

![My TB](https://github.com/semik/thunderbird-userChrome/blob/master/example.thunderbird.png)

## Plugins
