# FLASHBACK


Репозитарий движка Remeniscene
Код содержит правки через define позволяя отключить рендреринг тех или иных частей игры
Есть сохранения каждой комнаты 1го уровня
Исследуя Git историю можно понять какие модификации сделаны


Необходимые пакеты для запуска
brew install 
SDL2-dev
SDL2
sdl2_gfx
sdl2_image
sdl2_mixer
sdl2_ttf
libsdl2-dev
ibvorbisdec
libvorbis
libvorbis-dev
libvorbisidec
libvorbisidec-dev
tremor
libtremor
libogg
libvorbis
vorbis-tools
libtheora
libmodplug
libvorbisidec-dev
libvorbisidec

imagemagick




ffmpeg -framerate 57 -i seq_%05d.png -pix_fmt yuv420p  out.mp4

ffmpeg -i intro.mp4 -c:v libtheora intro.ogv

ffmpeg -i intro.mp4 -c:v libtheora -q:v 10  intro.ogv

ffmpeg -framerate 57 -i seq_%05d.png -pix_fmt yuv420p wakeup.mp4

ffmpeg -i wakeup.mp4 -c:v libtheora -q:v 10 wakeup.ogv


// Преобразовываем скриншоты игры в png
mogrify -format png *.bmp


// уникальные кадры
identify -format "%# %f\n" *.bmp | sort -u -k1,1 | cut -d' ' -f2



ffmpeg -ss 00:00:00 -i flashback-playback.mp4 -to 00:14:00 -c copy flashback-level1-playback.mp4

 
-i: This specifies the input file. In that case, it is (input.mp4).
-ss: Used with -i, this seeks in the input file (input.mp4) to position.
00:01:00: This is the time your trimmed video will start with.
-to: This specifies duration from start (00:01:40) to end (00:02:12).
00:02:00: This is the time your trimmed video will end with.
-c copy: for make in instantly. In that case ffmpeg will not re-encode video, just will cut to according size.



RESOURCES:

 
[Eng] Flashback - Death Scenes (Sega Genesis & CD) [1080p60][EPX+]
https://www.youtube.com/watch?v=-ndyOnPWVH8
 
Flashback - All Cutscenes (Game Movie)
https://www.youtube.com/watch?v=K043ZXbioWY

https://github.com/search?l=C%2B%2B&p=2&q=reminiscence&type=Repositories
 
https://github.com/chermenin/REminiscence  !!!!!!!!!!!!
https://github.com/Cheeseness/REminiscence
 
http://cyxdown.free.fr/reminiscence/flashback_cutscene.pdf
http://cyxdown.free.fr/reminiscence/flashback_3do.pdf
 
CUTSCENES!!!!!
http://cyxx.github.io/dpoly_js/
 
http://cyxdown.free.fr/reminiscence/