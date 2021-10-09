

    CATEGORY: web
    POINTS: 200
    DOWNLOAD LINK: None
    ACCESS: http://chal.ctf-league.osusec.org:31337/
    DESCRIPTION: Welcome to the OSUSEC CTF League! The goal of each of these challenges 
    is to find a flag that will be in the form osu{n0t_a_fL4g}. When you capture the flag, 
    submit it in this channel using $submit <flag>. To start, open the linked website in your browser. 
    Good luck!





  1.  We were given a link and upon reaching the site, we see this:


  ![Screenshot from 2021-10-09 03-22-01](https://user-images.githubusercontent.com/47869961/136654639-d7ed2ef5-dfb8-4237-8d60-f0ff5dee7b81.jpg)


  After reading through the paragraph, we inspected all the links given to us and knew that the link to
  **CrackStation** would be useful in the future once we were able to obtain the hash. At the end of the paragraph,
  it prompted us to inspect the "Submit" button.


  2.  Inspecting the "Submit" button gave us the source code for the HTML file where we were able to find 
  the hash code.
  
  Hash = "b0fef621727ff82a7d334d9f1f047dc662ed0e27e05aa8fd1aefd19b0fff312c"

  ![image](https://user-images.githubusercontent.com/47869961/136655093-0d17f4d6-3e77-4a8f-b18f-14b50fcd525a.png)
  
  3. Running the hash value through CrackStation gave us the result: "pineapple". Noticing that the
  has type was "sha256" that was referenced in the paragraph found on the first webpage, we made
  the connection that this was the login passphrase.

  ![image](https://user-images.githubusercontent.com/47869961/136655355-feb2c259-4372-492a-8b83-12eeca0f24cd.png)
  
  4. Once we got past the first page, we were sent to another page
  that had a link that was bouncing on the screen that read "Get the flag!". By inspecting the HTML source,
  we see that there is a command written in javascript that can be executed in the Console tab next to Inspector.
  Once we typed in "print_flag()", the page updated to the flag bouncing on the screen once again. Avoiding
  the annoyance of trying to chase the flag on the screen, we can find the flag in the HTML source file.
  
  ![image](https://user-images.githubusercontent.com/47869961/136655557-3f54b259-aa2c-4a4f-9d83-3610b8803363.png)
  
  5. osu{p1n34ppl3_h45h_Br0wN5_4r3_g00D}
