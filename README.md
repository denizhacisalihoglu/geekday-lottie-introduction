# geekday-lottie-introduction
In this repository, you can find 2 samples of lottie animation integration and after effects working files.

### Import Lottie Script
```
<script src="https://cdnjs.cloudflare.com/ajax/libs/bodymovin/5.7.7/lottie.min.js" type="text/javascript"></script>
```

### Run lottie animation

Create a container to load lottie animation into it
```
<div id="myLottie"></div>
```

Create lottie script
```
<script>
    lottie.loadAnimation({
          container: document.getElementById("myLottie"), 
          renderer: "svg",
          loop: true,
          autoplay: false,
          path: "https://assets9.lottiefiles.com/packages/lf20_2fWXlk.json",
    });
</script>
```
### Main methods of Lottie
| Method Name | Description |
| --- | --- |
| anim.play() | Plays lottie animations |
| anim.stop() |  Stops lottie animations |
| anim.pause() | Pauses lottie animations |
| anim.setSpeed(speed) | Sets speed of animation. Value is between 0-1 |
| anim.goToAndStop(value:numeric, isFrame:boolean) | isFrame(true:frame, false:time) |
| anim.goToAndPlay(value:numeric, isFrame:boolean) | isFrame(true:frame, false:time) |
| anim.setDirection(direction) | 1 is normal direction. -1 is reverse direction |
| anim.playSegments(segments, forceFlag) -- first param is a single array or multiple arrays of two values each(fromFrame,toFrame), second param is a boolean for forcing the new segment right away |
| anim.destroy() | destroys lottie animation |

### Resources
http://airbnb.io/lottie/

http://lottiefiles.com/
