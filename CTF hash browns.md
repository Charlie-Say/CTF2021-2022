

  CATEGORY: web
  POINTS: 200
  DOWNLOAD LINK: None
  ACCESS: http://chal.ctf-league.osusec.org:31337/
  DESCRIPTION: Welcome to the OSUSEC CTF League! The goal of each of these challenges 
  is to find a flag that will be in the form osu{n0t_a_fL4g}. When you capture the flag, 
  submit it in this channel using $submit <flag>. To start, open the linked website in your browser. 
  Good luck!





1.  We were given a link and upon reaching the site, we see this:


  ![Screenshot from 2021-10-09 03-22-01](https://user-images.githubusercontent.com/47869961/136654639-d7ed2ef5-   dfb8-4237-8d60-f0ff5dee7b81.jpg)

  
    After reading through the paragraph, we inspected all the links given to us and knew that the link to
    **CrackStation** would be useful in the future once we were able to obtain the hash. At the end of the paragraph,
    it prompted us to inspect the "Submit" button.
  
  
2.  Inspecting the "Submit" button gave us the source code for the HTML file where we were able to find 
    the hash code.
  
    ![image](https://user-images.githubusercontent.com/47869961/136655093-0d17f4d6-3e77-4a8f-b18f-14b50fcd525a.png)
