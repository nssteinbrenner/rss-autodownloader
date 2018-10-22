# rss-autodownloader
Automatically torrents from RSS feed based off of your specified targets.

Designed for videos, will require some modifying for other formats, namely the 'quality' field will have to be modified for certain other media that might not have a clear quality label.

Reads several parameters from a config file. Note the spaces, as they are essential for the program to properly parse the config file.

Config file:
quality: {video quality, e.g 1080 (omit the 'p' normally appended)}                                                                                                                        
feeds: {/path/to/feedsfile} (explained below)                                                                                                           
targets: {/path/to/targetsfile} (explained below)                                                                                                      
archive: {/path/to/archivefile} (explained below)                                                                      
fromaddr: {sender email addr}                                                                                                                        
toaddr: {recipient email addr} {recipient email addr 2} {etc...} (be sure to space seperate all email addresses)                                                                                                     
password: {sender email passwd}                                                                                                                            
torrentdir: {/path/to/torrentdirectory}

Targets file is simply the phrase you are looking for in the RSS feed, each phrase you are seeking is separated by a new line.

Targets  File:  
{show I like}  
{another show I like}  
{etc...}  

The feeds file contains the RSS feeds you'd like to search. Each RSS feed is separated by a new line.

Feeds file:  
{rss feed}  
{another rss feed}  
{etc...}  

Archive file is left blank, the program will automatically write to it. It solely exists so you do not download the same thing twice.
