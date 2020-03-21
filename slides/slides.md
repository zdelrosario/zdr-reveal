<!-- .slide: class="center" -->
# reveal.js slide deck

Zach del Rosario

<!-- ------------------------------ -->
<!-- ---------- OVERTURE ---------- -->
<!-- ------------------------------ -->

<------>
<!-- .slide: class="center" -->
### Setup

- Edit `zdr-reveal/slides/Makefile` to copy image dependencies
  - Make sure to point `IMG_DIR` to correct directory
- Run `$ make setup` to download and build presentation stack
- Run `$ make` to start reveal.js presentation
- Run `$ make deps` if you add new images

<------>
<!-- .slide: class="center" -->
### Slide formatting

- I prefer default top alignment
- Use `.slide: class="center"` per-frame for vertical centering

<------>
### Images

- `div` (overlay) placement works only with top-aligned slides

<img src="./img/tao_cropped_2018.png" alt="TAO 2018" align="middle" width="55%">

<div style="position: absolute; width: 35; top: 50%; left: 15%; box-shadow: 0 1px 4px rgba(0,0,0,0.5), 0 5px 25px rgba(0,0,0,0.2); background-color: rgba(0, 0, 0, 0.9); color: #fff; padding: 20px; font-size: 40px; text-align: left;">
Overlay
</div>
