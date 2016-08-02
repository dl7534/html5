# audio 对象身上的属性和方法
> 一个audio 对象就是普通的dom对想
> 比其他的dom对象多出一些自己独有的属性方法和事件
·······javascript	``````
  var acdio = $('audio').get(0);
`````````````````````````````
## 属性
   audio.volume  (读/写)  音量
   audio.src     (读/写)  歌曲地址

   audio.paused  (读/写)  boolean类型   是否处于暂停状态
   audio.ended    (读)    boolean类型   歌曲是否已经播放完毕

   audio.currentTime(读/写)      歌曲当前已播放的时长
   audio.duration (读)           歌曲的总长度
   

##方法
   audio.play()                  让歌曲开始播放
   audio.pause()                 让歌曲暂停
   audio.fastseek()              让歌曲来到指定的位置   // 暂时停用
##事件
    audio.oncanplay = fn()       当歌曲下载完之后的调用 fn
    audio.onvolumechange = fn()  当audio.volume 发生变换的时候调用 fn
    audio.onpause = fn()          歌曲暂停之后调用fn
    audio.ontimeupdate = fn()    歌曲在播放的过程中会一直调用fn
    audio.onplay = fn()          歌曲开始播放之后调用fn   
    audiio.onpause = fn()        歌曲暂停之后调用fn
    audio.onended = fn()         歌曲播放完之后调用fn



toFixed(2)


