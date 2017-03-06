The Nano CPS has several “flight modes” which are controlled using channel 5 (depending on your transmitter, this may be labelled as the “gear” or “gyro” channel).  By changing the value of channel 5, you can control how your CPS behaves, from mild-to-wild.  Here are the values for each mode alongside a description of their behavior.

I determined these values experimentally by mapping channel 5 to a knob on my Spektrum DX8G2 transmitter, and they range from a minimum value of -125% to a maximum of 125% … you may have to scale the values for other brands of transmitter that have different minimum / maximum limits.  Note that hitting exact values with the knob wasn’t easy, so I’ve recorded the boundaries between modes without trying to nail-down whether a given boundary value fell into one mode or another.  When programming your transmitter, you’ll want to use values near the middle of each range, so there’s no ambiguity about which mode you’re in. 

| Mode           | Low Value | High Value | LED Color | Behavior |
| -------------- | --------- | ---------  | --------  | -------- |
| Stability Mode | 15%       | 125%       | Blue | Attitude control. |
| Agility Mode   | -15%      | 15%        | Red | No attitude control, mild responsiveness. |
| Panic Mode     | -85%      | -15%       | Blue | Attitude control. |
| 3D Mode        | -115%     | -85%       | Red | No attitude control, aggressive responsiveness. |
| Panic Mode     | -125%     | -115%      | Blue | Attitude control. |

Here’s how you can map these values to your transmitter: assign a three-position switch to channel 5 and program values of 100% (stability mode), 0% (agility mode), and -100% (3D mode).  Then use programmable mixing and a push button or a two-position switch to subtract 20% when activated, resulting in 80% (you’re still in stability mode), -20% (panic mode) and -120% (panic mode), respectively.
