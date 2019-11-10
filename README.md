# voce_tem_um_momento_para_falar_sobre_o_github
 Com licença, você tem um momento para falar sobre o github


Animate Xaringan Slide Transitions
https://www.garrickadenbuie.com/blog/animate-xaringan-slide-transitions/

download.file(
  "https://raw.githubusercontent.com/daneden/animate.css/master/animate.css",
  "animate.css"
)


and then list animate.css in the css YAML section.

output:
  xaringan::moon_reader:
    lib_dir: libs
    css: [default, default-fonts, animate.css]

Or if you’ll have reliable internet during your presentation you can link directly to a CDN.

output:
  xaringan::moon_reader:
    lib_dir: libs
    css:
      - default
      - default-fonts 
      - "https://cdnjs.cloudflare.com/ajax/libs/animate.css/3.7.0/animate.min.css"