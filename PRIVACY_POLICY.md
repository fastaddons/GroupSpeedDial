## TLDR:
- I'm doing my best to protect your data
- your data are not shared with any 3rd party
- without cloud account your dials data stays local
- all server requests always contains minimum required info, never personal or any tracking data
- addon development is fully financed through Patreon and donations (thank you!)


# Privacy Policy
Group Speed Dial allows you to backup and synchronize your dials using "Cloud server" at https://group-speed-dial.fastaddons.com/
  
If you create a cloud account there, your dials data will be synchronized with the Cloud server.  
These data contains only basic information (entered by you) about your dials - such as name, URL, note, date created, crop / scale, custom settings, visual settings, etc...  
There are NO tracking data nor statistics!  
No personal information is being collected nor transferred!  
  
Example data send to cloud server representing single group with single dial:    
"{"groups": [[0, "Home group", 3, 4, [["Internet for people, not profit — Mozilla", 0, "https://www.mozilla.org/en-US/", 0, [0, 0, 1, 0, 0], 0, 0, 0, 25680324], 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0], 0, "rgb(255, 0, 0)", 0]], "sync": {}}"  
  
Since version 11.2 you will be able to synchronize your thumbnails with your cloud account. Thumbnails synchronization is disabled by default and needs to be enabled in Options page by checking "Enable automatic thumbnails synchronization with the cloud server". Thumbnails uploaded to the cloud server are private and only users with the full URI link can access them.  

Since version 11.2 you will be able to upload individual thumbnails to the public library and make it available to everybody. You can make thumbnail public by invoking context menu on a dial / "Advanced" / "Upload thumbnail to public library". You will be asked to confirm your action. Data send to the server contains - the thumbnail, dial name and thumbnail position (center, full width, cover or fill). Other users will not know, who uploaded the thumbnail.  
  
Cloud server is hosted at https://www.tilaa.com/ VPS provider in Netherlands (Europe). All data transfers are made using encrypted HTTPS connections. Access to the cloud server (and thus users data) has only author of this add-on: Ing. Juraj Mäsiar.  
  
Sub-domain pages of "fastaddons.com" can detect that you have this add-on installed - this is used to display "Return back to extension" button on "group-speed-dial.fastaddons.com" after you create a cloud account.  
Web-page "https://maketext.io/" opened through this add-on (from the "Edit dial" window / Thumbnail tab / "Create your own Text Thumbnail using web-page MakeText.io" / "Open page" button) can detect that you have this add-on installed. This is due to integration with this service to allow creation of custom text thumbnails. The web-page receives only current dial name, no other information is transferred.  
  
  
**Without cloud account, your dials data stays on your PC!**  
  
Using cloud related features can create requests to the Cloud server:  
1) if you create new dial for "some_domain.com" page, the favicon is downloaded directly from that page - "some_domain.com/favicon.ico". If the page specifies a different path for favicon in its HTML, such favicon is again directly downloaded. If no favicon can be found on the page, the addon will contact Cloud server for favicon. This request contains only domain name for which the favicon is requested.

3) Since version 11.2 you will be able to use load thumbnails for your dials from public library - hosted on the cloud server. If you select "Thumbnail from public library:" and then click "Load images", request will be send to my server to load list of thumbnails available for requested domain. The request contains only domain name (for which the thumbnails are requested).  
  
4) Since version 12.3 you are able to use backgrounds from Bing.com page - the "Bing's image of the day". When this is enabled in Options page / Background, my add-on will make simple image request to bing.com domain to fetch new image every day. No private information are being sent!  
  
## See also:
🏠 [Wiki Home](https://github.com/fastaddons/GroupSpeedDial/wiki)  
🚩 [Permission justification](https://github.com/fastaddons/GroupSpeedDial/blob/master/PERMISSION_JUSTIFICATION.md)
