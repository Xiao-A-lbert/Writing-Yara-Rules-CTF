# Writing-Yara-Rules-CTF

<h2>Description</h2>
In this Threat Intelligence task, I create multiple yara rules that include strings, registry keys, and file signatures to answer the CTF questions. 

<h2>Languages and Utilities Used</h2>

- <b>YARA</b>
- <b>Linux CLI</b>

<h2>Environments Used </h2>

- <b>Ubuntu</b> 

<br />
<br />
Challenge prompt.

![1) challenge prompt](https://github.com/user-attachments/assets/86ae7aac-eeea-428d-9e04-f8a204589ef5)

<br />
<br />
Finding the jpg string within HawkEye.exe.meow.

![2) jpeg](https://github.com/user-attachments/assets/02faeaee-3f73-499e-b938-028e1057aaaf)

<br />
<br />  
Writing a yara rule for that specific jpg in HawkEye.exe.meow. 

![3) yara rule](https://github.com/user-attachments/assets/2237ac4e-cacf-4e3b-bd87-09cbbf4094ba)

<br />
<br />
Running the yara rule and outputting the offset location of the matching detection. 

![4) q2](https://github.com/user-attachments/assets/f1bcb1fe-6ab5-44a1-9e28-6d50231f91cc)

<br />
<br />
Running the provided rule1.yar against the entire Samples directory and outputting the detected files and printing the matched strings. 

![5) q4 5](https://github.com/user-attachments/assets/2e71169f-6827-4144-8d49-c9c20720ab40)

<br />
<br />
youtubedownloadernew[.]com is the base domain name in the FreeYoutubeDownloader.exe.meow file. 

![6) q 6](https://github.com/user-attachments/assets/d81c081e-ae6d-4ed6-b6d7-2364ec1f2832)

<br />
<br />  
Creating and running a yara rule from the youtubedownloadernew[.]com base domain name against the FreeYoutubeDownloader.exe.meow file to print out the hexadecimal offsets of the two matching strings. 

![7) q7](https://github.com/user-attachments/assets/aa473c9e-3423-4a58-be1c-e49dd1a42c61)

<br />
<br />  
Searching for the host artifact of SOFTWARE\BORLAND\DELPHI\RTL within the FreeYoutubeDownloader.exe.meow file.
    
![8) q8](https://github.com/user-attachments/assets/9f3d3003-9485-487b-9102-ced0838d47f3)

<br />
<br />
Create and run  recursively a new yara rule containing the host artifact against the FreeYoutubeDownloader.exe.meow file. to show 2 other files detecting the host artifact. 
    
![9) double back slash for escaping](https://github.com/user-attachments/assets/750a0294-d638-4881-a439-49ef230e06bf)

<br />
<br />  
The yara rule created with the host artifact, make sure to use double \\ to properly write the string.. 

![9 1) rule](https://github.com/user-attachments/assets/ce95e215-1d31-4c74-aed6-c6e65b956215)

<br />
<br />  
The yara rule created to find OpenSSH file signatures for private keys within a portable executable. 
    
![11) exe open ssh file signature rule](https://github.com/user-attachments/assets/379ac21d-9d0e-4341-bdca-2127f297838b)

<br />
<br />
Running the openssh private key PE yara rule shows two matching files. 
    
![12) file detected](https://github.com/user-attachments/assets/d15654b8-9db1-489a-9386-b7f25e19a0c1)

<br />
<br />  
