# Q1&Q2.  
You can find the answers in the text mail.  
![06_0](https://user-images.githubusercontent.com/39981286/159650511-177f8cac-6b5b-4167-9aa4-8346b49b060a.jpg)  
![06_1](https://user-images.githubusercontent.com/39981286/159651897-77269c44-40c7-4884-98a2-1dcda2df9425.jpg)  

# Q3.  
I couldn't open the attachement because of the decode failure from the mail included the zip, so I needed to use web site here (https://base64.guru/converter/decode/file)  
And it's the very point that you should convert to file(zip) not to pdf. If you convert to pdf, you cannot read the pdf file output even if you use Adobe software or web browser.  

\# unzip application.zip  
Now, you can see a new directory "PuzzleToCoCanDa".  

\# cd PuzzleToCoCanDa && ls -l  
-rwxrwxrwx 1 kali kali 18662 Jan 25  2021  DaughtersCrown  
-rwxrwxrwx 1 kali kali 28475 Jan 26  2021  GoodJobMajor  
-rwxrwxrwx 1 kali kali 16541 Jan 26  2021  Money.xlsx  
As you know, you can open .xlsx by Microsoft software Excel, and you will find a message from them.  
But be careful to show full space each cells. You need to click a button at the top of the bar.  

Let's take a look other files.  
\# file DaughtersCrown
DaughtersCrown: JPEG image data, JFIF standard 1.01, resolution (DPI), density 120x120, segment length 16, baseline, precision 8, 822x435, components 3  
\# file GoodJobMajor
GoodJobMajor: PDF document, version 1.5, 1 pages  
DaughtersCrown looks like .JPEG file and I renamed this file and open. I could see a illustration of Crown.  
 ![06_3_small](https://user-images.githubusercontent.com/39981286/159651488-a2cf5556-3f9b-4972-b04b-66d745567789.jpg)  

GoodJobMajor looks like .pdf file and I rename this file and open.  
![06_4_small](https://user-images.githubusercontent.com/39981286/159651500-47a2901a-e7a6-481f-b906-2c7dbaee213f.jpg)  

# Q4.    
I investigated each file...  
\# exiftool GoodJobMajor  
I could find a person's name. That's an author, perhaps one of the answers.  

# Q5.  
I couldn't figure out any contents in the second sheet, "Sheet3", so I exported to a text file from xlsx file format.  
Then I can see a message inside sheet3.  
VGhlIE1hcnRpYW4gQ29sb255LCBCZXNpZGUgSW50ZXJwbGFuZXRhcnkgU3BhY2Vwb3J0Lg==  
It's base64, so I converted it using here (https://www.base64decode.org/) and got a true message.  

# Q6.  
You can get from the first text mail as well.  

answers:
Q1) emkei.cz
Q2) negeja3921@pashter.com
Q3) .zip
Q4) Pestero Negeja
Q5) The Martian Colony, Beside Interplanetary Spaceport
Q6) pashter.com  

references:  
https://base64.guru/converter/decode/file  
https://www.base64decode.org/  
https://medium.com/cryptogennepal/the-planets-prestige-blue-team-labs-online-walkthrough-770a1c13936b  

