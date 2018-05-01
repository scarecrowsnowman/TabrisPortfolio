# TabrisVideo Tutorial
This is a small video play function of this app in Tabris for my portfolio, will be base on JavaScript. 

![](https://github.com/scarecrowsnowman/tabrisportfolioo/blob/master/img/7.jpg?raw=true)

The picture above will be what the application looks like. 

When you try to add a video the following code is what you need:

let video = new Video({
  left: 100, top: 70, right:100, bottom: '#button3 16', 
  url: 'https://github.com/scarecrowsnowman/imd-learning-tabris/raw/master/images/121.mp4',
  controlsVisible: true
}).on('select', () => video.state === 'play' ? video.pause() : video.play())
  .appendTo(ui.contentView);
