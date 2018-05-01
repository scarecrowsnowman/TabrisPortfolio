# TabrisVideo Tutorial
This is a small video play function of this app in Tabris for my portfolio, will be base on JavaScript. 

![](https://github.com/scarecrowsnowman/tabrisportfolioo/blob/master/img/7.jpg?raw=true)

The picture above will be what the application looks like. 

When you try to add a video the following code is what you need:<br />

"let video = new Video({<br />
url: 'https://github.com/scarecrowsnowman/imd-learning-tabris/raw/master/images/121.mp4',<br />
}).on('select', () => video.state === 'play' ? video.pause() : video.play())<br />
  .appendTo(ui.contentView);"<br />

If you want to move the position you should include the: <br />
left: 100, top: 70, right:100, bottom: '#button3 16'<br />
for the second line. <br />

controlsVisible is a function which would show the control panel, if you want to see the panel you should set it to "true", if you don't want to see the panel you should set to false. ![](https://github.com/scarecrowsnowman/tabrisportfolioo/blob/master/img/2.png)

Right now the final code for this video show looks like this:<br />
let video = new Video({<br />
left: 100, top: 70, right:100, bottom: '#button3 16', <br />
url: 'https://github.com/scarecrowsnowman/imd-learning-tabris/raw/master/images/121.mp4',<br />
controlsVisible: true<br />
}).on('select', () => video.state === 'play' ? video.pause() : video.play())<br />
.appendTo(ui.contentView);<br />

Sometimes your video.state would be replaced like the following code:<br />

![](https://github.com/scarecrowsnowman/tabrisportfolioo/blob/master/img/4.png)

This would cause error and it would show in your console:
![](https://github.com/scarecrowsnowman/tabrisportfolioo/blob/master/img/6.jpg)

If your code looks like this:
![](https://github.com/scarecrowsnowman/tabrisportfolioo/blob/master/img/1.png)
You are not going to have any trouble!
