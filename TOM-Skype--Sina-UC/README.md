Overview 
========

TOM-Skype was the Chinese version of Skype until 2013. Sina UC was a chat client provided by Sina Corporation, the operators of the Sina Weibo microblogging platform. For a period of more than a year and a half, we downloaded and decrypted the censorship and surveillance keywordlists used by TOM–Skype and Sina UC. We obtained the keyword list URLs and encryption keys by reverse engineering the software binaries of the clients. In the TOM–Skype client, keyword lists were used to trigger censorship and/or surveillance of user chats, while in Sina UC the keyword lists trigger only censorship. This data affords a rare opportunity to analyze the contents of, and updates to, complete and unbiased keyword lists used for both censorship and surveillance. 

Note that since November 2013, Microsoft is no longer partnering with TOM and now partners with GMF to bring Skype to China. Unlike TOM-Skype, we have not found GMF-Skype to have any additional censorship or surveillance capabilities built into the software. However, since no version of Skype provides true end-to-end encryption that Microsoft cannot decrypt, Microsoft is still theoretically capable of performing censorship or surveillance of anyone's Skype communication as it passes through their servers.

Data
========
Collection of the keyword lists began on 24 April 2011 (TOM–Skype)/8 August 2011 (Sina UC) and ended on 31 January 2013, with the latest changes occurring on 20 December 2012 (TOM–Skype)/11 October 2012 (Sina UC). In total, the dataset consists of 88 lists, which combined contain 4,256 unique keywords. Keywords were translated to English using combination of machine and human translation. Based on interpreting these translations with contextual information, we coded each keyword into content categories grouped under six general themes according to a code book

Note that raw collection data is available in directories ending in \*-raw-data.  Each file represents an observed update to a list, as measured via daily collection at 6pm UTC (2am the next day China Standard Time), and contains the contents of the list at that time indicated by the file's name.  For instance, [tom-skype-raw-data/dlist-5.5s/keyfile_u.2013-06-18.plain](https://github.com/citizenlab/chat-censorship/blob/master/TOM-Skype--Sina-UC/tom-skype-raw-data/dlist-5.5s/keyfile_u.2013-06-18.plain) is TOM-Skype 5.5's Surveillance-only list on June 18 2013 6pm UTC.

Resources 
========
For decryption scripts see [Jeffrey Knockel's webpage](https://www.cs.unm.edu/~jeffk/tom-skype/).

For details on reverse engineering methods and results see
[Three Researchers, Five Conjectures: An Empirical Analysis of TOM-Skype Censorship and Surveillance](https://www.cs.unm.edu/~jeffk/publications/foci11tomskype.pdf) and [Chat program censorship and surveillance in China: Tracking TOM-Skype and Sina UC](http://firstmonday.org/ojs/index.php/fm/article/view/4628/3727).

[Explore visualizatons of the data](https://china-chats.net).
