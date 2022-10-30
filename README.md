# Social Media Blocker Chrome Extension

## This chrome extension blocks social media sites and helps you focus on your work without getting distracted.

### Currently Blocked sites:
  1. Youtube
  2. Facebook
  3. Netflix
  4. Instagram
  5. Twitter
  6. Whatsapp
  
 ### Steps to install this extension on your browser
 1. Clone this repository or download it as a zip on your local system.
 2. Open chrome and click on the extensions button (looks like a piece of jigsaw puzzle).
 3. Select Manage Extensions option which will open Extensions tab on chrome.
 4. Turn on Developer mode (on the top right corner) 
 4. Click on the Load Unpacked button (on top left corner).
 5. A pop-up window will open in which you will have to select the Extension's folder location.
 6. Make sure that the extension is turned on and has access to all the sites (see 3 dot menu of the extension or details)
 
Congratulations!!! You now have a working chrome extension which will block all the distracting websites.

### Steps to add more sites to the block list
1. Open Content.js file and go to bottom of it.
2. copy paste a case before the closing curly bracket  
      case "web.whatsapp.com":  
       document.head.innerHTML = generateSTYLES();  
       document.body.innerHTML = generateHTML("WhatsApp");  
       break;  
3. just change the domain name and arguement in generateHTML function and save the file.
4. refresh the extension in chrome's extension tab.
