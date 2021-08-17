

<p align="center">
  
  <img src="https://media.giphy.com/media/2tSMdSUTtrrrCwD5VK/giphy.gif" width="200"/>

</p>
<br>
<img src="https://yata-apix-a9caea66-ad78-425f-aa08-e292558ebb65.lss.locawebcorp.com.br/b7c7dbff38ae4f419c94ce8d2254b9d9.png"> 

=> ADS Student for love<br>
=> Ph.D Student in oncology area - Yes, I'm crazy ¯\(°_o)/¯ 

=> Code Learner
  - Python ❤️  
  - HTML/CSS/JS 🤩

=> Tech Lover 💻

=> Data Science enthusiast 📊
  - Learnig Numpy, pandas, matplotlib (repositories soon)
  - Future plans: R, machine learning
  
 
 About me:<br>
  Hello my name is Saulo, 30 years old and live in Brazil / São Paulo. 
  
  Games:<br>
    - LOL<br>
    - RTS games<br>
    - RetroGames (SNES is my favorite console <3)
    
   Pets:<br>
    - Dog named Felipe Roberto 🐶
    
   Music:<br>
    - Almost all kinds
    
   <img src="https://yata-apix-a9caea66-ad78-425f-aa08-e292558ebb65.lss.locawebcorp.com.br/b7c7dbff38ae4f419c94ce8d2254b9d9.png"> 
        
  <h2>
   <p align="center">
  Do you have 5 minutes to talk about anything?<br>
  </p>
  </h2>



<h3 align="center">Connect with me:</h3>
<p align="center">
<a href="https://twitter.com/saulodetp" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/twitter.svg" alt="saulodetp" height="30" width="40" /></a>
<a href="https://linkedin.com/in/saulodetp" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/linked-in-alt.svg" alt="saulodetp" height="30" width="40" /></a>
<a href="https://fb.com/saulodetp" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/facebook.svg" alt="saulodetp" height="30" width="40" /></a>
<a href="https://instagram.com/saulodetp" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/instagram.svg" alt="saulodetp" height="30" width="40" /></a>
<a href="https://medium.com/@saulodetp" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/medium.svg" alt="@saulodetp" height="30" width="40" /></a>
</p>


<p align="center">
<img align="center" src="https://github-readme-stats.vercel.app/api?username=saulotp&show_icons=true&locale=en" alt="saulotp" />
</p>

name: Generate Datas

on:
  schedule: # execute every 12 hours
    - cron: "* */12 * * *"
  workflow_dispatch:

jobs:
  build:
    name: Jobs to update datas
    runs-on: ubuntu-latest
    steps:
      # Snake Animation
      - uses: Platane/snk@master
        id: snake-gif
        with:
          github_user_name: saulodetp
          svg_out_path: dist/github-contribution-grid-snake.svg

      - uses: crazy-max/ghaction-github-pages@v2.1.3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
