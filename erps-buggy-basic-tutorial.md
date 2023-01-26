### @activities true
### @explicitHints true

# ERPS STEM WEEK :: Motorised Buggy - Starter

## Introduction
### Introduction Step @unplugged
The motorised buggy - possibly the coolest of our STEM challenges!  
  
This buggy is capable of loads of cool things, but let's start slowly, and build up our confidence!  
  
**Q. What are we using to power our buggy?**  
**Q. What alternative power sources are there, and is this the best?**
  
In this tutorial, we're going to begin by making our buggy go forwards and backwards, using the buttons on our micro:bit.

![Motorised Buggy](https://raw.githubusercontent.com/niaxotim/erps-buggy-basic-movement/master/assets/buggy.png)

## Putting our buggy together!
### Assembling the pieces @unplugged
Before we start, make sure your buggy has been assembled. There are lots of sensors we *can* connect, but for now, just make
sure that the tyres are on the wheels, and that the wheels are connected to the motors.  
  
Oh, and don't forget some AA batteries too!

![Buggy Key Features](https://raw.githubusercontent.com/niaxotim/erps-buggy-basic-movement/master/assets/features.png)


## Let's get moving!
### Step 1
OK, we're starting simple. So let's try and get our buggy to go forwards. We're going to make this happen
when we press our 'A' button.  

We also need to choose how fast. The speed ranges from 0 to 100.  Let's try 30 for now... so we don't have to run after our buggy ;)

Let's start with a ``||input:on button A||`` block.

#### ~ tutorialhint
```blocks
input.onButtonPressed(Button.A, function () {
})
```

### Step 2
Now drag a ``||Kitronik_Move_Motor.Move Forward at Speed 0||`` block, then change the speed to 30.  
  
#### ~ tutorialhint
```blocks
input.onButtonPressed(Button.A, function () {
    Kitronik_Move_Motor.move(Kitronik_Move_Motor.DriveDirections.Forward, 30)
})
```

### Step 3
Great! So now our buggy will go forwards. But what about going backwards?  

Can you get the buggy to travel backwards when you press the 'B' button instead? Don't forget to set the speed! ;)  
  
#### ~ tutorialhint
```blocks
input.onButtonPressed(Button.B, function () {
    Kitronik_Move_Motor.move(Kitronik_Move_Motor.DriveDirections.Reverse, 30)
})

```

### Step 4
Now our buggy goes backwards, and forwards. But you must be running after it all of the time!  
  
How do we make it stop? Well, there's a neat ``||Kitronik_Move_Motor.Stop||`` block for that!  
  
Let's add some code to make our buggy stop when we press 'A and B' at the same time.

#### ~ tutorialhint
```blocks
input.onButtonPressed(Button.AB, function () {
    Kitronik_Move_Motor.stop()
})
```

### Step 5
Connect your BBC micro:bit and click ``|Download|`` to transfer your code.  

Put your micro:bit in to the slot on the buggy, and make sure that your buggy is switched on.  

Now try pressing 'A', 'B', and 'A and B'. Does your buggy move as expected?  

Do you notice anything when the buggy stops? Check out the back for a hint ;)

### Motorised Buggy Basic Tutorial Complete @unplugged
Great work! You've just coded your first functions for your buggy! Now you're really motoring ;). 

![Great job](https://raw.githubusercontent.com/niaxotim/erps-buggy-basic-movement/master/assets/great_job.png)
