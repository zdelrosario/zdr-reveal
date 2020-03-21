IMG_DIR=../images

serve:
	cd reveal.js; npm start

getjs:
	git clone git@github.com:hakimel/reveal.js.git
	cd reveal.js; npm install; npm audit fix
	mkdir reveal.js/img

cpmats:
	cp index.html reveal.js/.
	cp custom.css reveal.js/css/theme/.
	cp monokai.css reveal.js/lib/css/.

getjump:
	git clone git@github.com:SethosII/reveal.js-jump-plugin.git
	cp -r reveal.js-jump-plugin/jump reveal.js/plugin/.

setup:
	make getjs
	make cpmats
	make deps
	make link
	make getjump

link:
	ln -f slides.md reveal.js/slides.md

deps:
	ln -f ${IMG_DIR}/tao_cropped_2018.png reveal.js/img/.

clean:
	rm -fr reveal.js
	rm -fr reveal.js-jump-plugin
