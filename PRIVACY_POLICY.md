# Privacy Policy

Group Speed Dial allows you to backup and synchronize your dials using cloud server at https://group-speed-dial.fastaddons.com/
  
If you create a cloud account there, your dials will be synchronized with this server.  
These data contains only basic information (entered by you) about your dials - such as name, URL, note, date created, crop / scale, custom settings, visual settings, etc...  
There are NO tracking data nor statistics!  
No personal information is being transferred!  
  
Example data send to cloud server representing single group with single dial:    
"{"groups": [[0, "Home group", 3, 4, [["Internet for people, not profit — Mozilla", 0, "https://www.mozilla.org/en-US/", 0, [0, 0, 1, 0, 0], 0, 0, 0, 25680324], 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0], 0, "rgb(255, 0, 0)", 0]], "sync": {}}"  
  
Since version 11.2 you will be able to synchronize your thumbnails with your cloud account. Thumbnails synchronization is disabled by default and needs to be enabled in Options page by checking "Enable automatic thumbnails synchronization with the cloud server". Thumbnails uploaded to the cloud server are private and only users with a full URI link can access them (if your internet provider is monitoring your traffic, he will be able to access your thumbnails!).  

Since version 11.2 you will be able to upload individual thumbnails to the public library and make it available to everybody. You can make thumbnail public by invoking context menu on a dial / "Advanced" / "Upload thumbnail to public library". You will be asked to confirm your action. Data send to the server contains - the thumbnail, dial name and thumbnail position (center, full width, cover or fill). Other users will not know, who uploaded the thumbnail.  
  
Cloud server is hosted at https://www.tilaa.com/ VPS provider. All data transfers are made using encrypted HTTPS connections. Access to the cloud server (and thus users data) has only author of this add-on: Ing. Juraj Mäsiar.  
  
Sub-domain pages of "fastaddons.com" can detect that you have this add-on installed - this is used to display "Return back to extension" button after you create a cloud account.  
Web-page "https://maketext.io/" opened through this add-on (from the "Edit dial" window when creating custom text thumbnail) can detect that you have this add-on installed. This is due to integration with this service to allow creation of custom text thumbnails. The web-page receives only dial name, no other information is being transferred.  
  
  
Without cloud account, this add-on will NOT make any requests to any server!  
  
Only exceptions are:  
1) if you enable downloading of Favicons from Google service - in Options page, using checkbox "Enable usage of Google service to get Favicons for dials (used only when favicon cannot be downloaded directly)". In such case, this add-on will make requests to Google server to download Favicons. There requests are made only if favicon cannot be downloaded directly and this request happens only when creating thumbnail.  
  
2) Since version 11.2 you will be able to use load thumbnails for your dials from public library - hosted on the cloud server. If you select "Thumbnail from public library:" and then click "Load images", request will be send to my server to load list of thumbnails available for requested domain. The request contains only domain name (for which the thumbnails are requested). No private information are being sent!  
  
3) Since version 12.3 you are able to use backgrounds from Bing.com page - the "Bing's image of the day". When this is enabled in Options page / Background, then my add-on will make requests to bing.com domain to fetch new image every day. No private information are being sent!  
  
## Users data synchronized with the server
If user creates cloud server account, his data will be synchronized with the cloud server.  
These data are transmitted through secure HTTPS connection.  
Data are stored on the cloud server hosted at Tilaa.com service.  
No other 3rd party has access to users data.  
To put it in simple words - me, Juraj Mäsiar, author of Group Speed Dial, am the only person with access to the cloud server. Nobody else can access it (except for the provider itself - Tilaa.com). I'm doing my best to protect your data.  

