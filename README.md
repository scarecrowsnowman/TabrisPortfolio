# TabrisVideo Tutorial
This is a small video play function of this app in Tabris for my portfolio, will be base on JavaScript. 

![](https://github.com/scarecrowsnowman/tabrisportfolioo/blob/master/img/7.jpg?raw=true)

The picture above will be what the application looks like. 

When you try to add a video the following code is what you need:

"let video = new Video({
url: 'https://github.com/scarecrowsnowman/imd-learning-tabris/raw/master/images/121.mp4',
}).on('select', () => video.state === 'play' ? video.pause() : video.play())
  .appendTo(ui.contentView);"

If you want to move the position you should include the: 
left: 100, top: 70, right:100, bottom: '#button3 16'
for the second line. 

controlsVisible is a function which would show the control panel, if you want to see the panel you should set it to "true", if you don't want to see the panel you should set to false. 

Right now the final code for this video show looks like this:
let video = new Video({
left: 100, top: 70, right:100, bottom: '#button3 16', 
url: 'https://github.com/scarecrowsnowman/imd-learning-tabris/raw/master/images/121.mp4',
controlsVisible: true
}).on('select', () => video.state === 'play' ? video.pause() : video.play())
.appendTo(ui.contentView);
