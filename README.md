# NahamconCTF2022WriteUp

## **NAHAMCON CTF 2022 A WILD RIDE WRITEUP**

This is Forensic challenge;

![](https://i.imgur.com/Ii7wR6N.png)


I googled about gpx and found that it contains longitude and latitude location data including waypoints, routes and tracks.

There is a .zip file called gpx.zip but it is an encrypted file.I need to decrypt the .zip file first to see what's inside.


* Now our first step will be to get a hashes of the zip file using the zip2john tool.Now our work has become very easy as you can see that just we need to give the location of the saved hash and it will try its own dictionary to crack the password of the zip file through the hash.


1. ![](https://i.imgur.com/pPbVT9x.png)




* As seen in the photo below, the password of the zip file is crackme.
2. ![](https://i.imgur.com/jyLM0oG.png)

* We unzip our file and we see that it extracts too many gpx files.

3. ![](https://i.imgur.com/GjIV3vB.png)


* I researched how to view this file on the internet and found a tool called gpx viewer.

4. ![](https://i.imgur.com/nvfDlN5.png)

* After clicking on the file and saying open, I selected all the files with the gpx extension and said open. Green roads appeared on the map and our flag was there.

5. ![](https://i.imgur.com/86OszhS.jpg)

`flag{gpx_is_cool}`, Thank you for reading.
