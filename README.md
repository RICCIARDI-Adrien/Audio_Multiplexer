# Audio multiplexer

A simple passive multiplexer providing :
* two 3.5mm jack inputs connected to two PC line outputs,
* two 3.5mm jack outputs connected to active speakers and a headset,
* one 3.5mm jack input connected to the headset microphone,
* two 3.5mm jack outputs connected to two PC microphone inputs.

```
                      +------+
             Line out |      | Mic in
     +----------------| PC 1 |<---------------+
     |                |      |                |
     |                +------+                |
     |                                        |
     |                +------+                |
     |       Line out |      | Mic in         |
     |   +------------| PC 2 |<-----------+   |
     |   |            |      |            |   |
     |   |            +------+            |   |
     |   |                                |   |
     v   v                                |   |
  +----------------------------------------------+             
  |              AUDIO MULTIPLEXER               |
  |                                              |
  |  Audio             Audio                Mic  |
  |   in                out                 in   |
  |                                              |
  +----------------------------------------------+
                       |  |                  ^
                       |  |                  |
                +------+  +-----+   +--------+
                |               |   |
                v               v   |
           +----------+      +---------+
           |          |      | Headset |
           | Speakers |      |  with   |
           |          |      |  mic    |
           +----------+      +---------+
```

The multiplexer microphone input is designed to be driven separately in case this is needed later.
