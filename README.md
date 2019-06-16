# LiveLab
Experiments at [McMaster's LiveLab](https://livelab.mcmaster.ca)

## Liine Lemur interface
This interface is built for sampling and playing back sounds using [Liine's Lemur](https://liine.net/en/products/lemur/).

### OSC Configuration
Buttons have value of 0 or 1
```
/RecordButton1/x
/RecordButton2/x
/RecordButton3/x
/RecordButton4/x
/PlayButton1/x
/PlayButton2/x
/PlayButton3/x
/PlayButton4/x
```

Sample levels (0->1 float)
```
/Sample1/x
/Sample2/x
/Sample3/x
/Sample4/x
```

Room Reverb (0->1 float)
```
/RoomLevel/x
/StageLevel/x
/RoomReflection/x
/StageReflection/x
/Time/x
```

Spatialization for samples (0->1 float)
```
/Sample1Space/x
/Sample1Space/y
/Sample2Space/x
/Sample2Space/y
/Sample3Space/x
/Sample3Space/y
/Sample4Space/x
/Sample4Space/y
```

### Testing
Use [SuperCollider](https://supercollider.github.io) (port 57120) and set:
```
OSCFunc.trace(true);
```
