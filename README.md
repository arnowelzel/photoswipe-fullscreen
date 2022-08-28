# Fullscreen for PhotoSwipe

This plugin adds a fullscreen display buttun to the UI to [PhotoSwipe 5](https://github.com/dimsemenov/PhotoSwipe) by Dmytro Semenov. In addition to clicking the button you can also press the [F] key to enter fullscreen mode.

## Using the plugin

To use the plugin, import the module and create the plugin using the lightbox instance as parameter before you init the lightbox.

```
<script type="module">
import PhotoSwipeLightbox from 'photoswipe/dist/photoswipe-lightbox.esm.min.js';
import PhotoSwipeFullscreen from 'photoswipe-fullscreen/photoswipe-fullscreen.esm.min.js';

const lightbox = new PhotoSwipeLightbox({
  gallerySelector: '#gallery',
  childSelector: '.pswp-gallery__item',
  pswpModule: () => import('photoswipe/dist/photoswipe.esm.js'),
});

const fullscreenPlugin = new PhotoSwipeFullscreen(lightbox);

// make sure you init photoswipe core after plugins are added
lightbox.init();
</script>
```
