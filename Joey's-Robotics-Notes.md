# Preamble

Hi y'all it's me, Joey from the class of 2024, let me introduce what this doc is before you jump right into it.

This doc is my personal notes that I assembled throughout the 2023-2024 season as the programming lead. This doc is mostly organized chronologically, but should also be organized in a somewhat sane way. This doc starts at the beginning of the season, created in mid October of 2023. Most of these notes were for my personal learning and grappling with what the task of programing entailed and what needed to go into it. In the offseason I also started helping out with the middle school's programming team, and I started taking notes on what we did and goals for every week.

> As I am reformatting this into markdown, I'll leave some comments in blockquotes (like this) to hopefully clear some stuff up.

---
# Robotics stuff

> This is real early days here
> I had never been a part of a robotics team before this, so I had a lot to learn
> Please excuse me if some of this here at the begining is a little naive

Pg 42 of Game Manual Pt 1

[https://www.firstinspires.org/resource-library/ftc/technology-information-and-resources](https://www.firstinspires.org/resource-library/ftc/technology-information-and-resources)

Programming guide

[How to write an OpMode](https://ftc-docs.firstinspires.org/en/latest/programming_resources/tutorial_specific/android_studio/creating_op_modes/Creating-and-Running-an-Op-Mode-%28Android-Studio%29.html)

[FTC java documentation](https://javadoc.io/doc/org.firstinspires.ftc)

[https://github.com/SLHS-Robotics/SLHS-Offseason-2024](https://github.com/SLHS-Robotics/SLHS-Offseason-2024)

[https://github.com/FIRST-Tech-Challenge/FtcRobotController](https://github.com/FIRST-Tech-Challenge/FtcRobotController)

[https://ftc-docs.firstinspires.org/en/latest/programming_resources/index.html](https://ftc-docs.firstinspires.org/en/latest/programming_resources/index.html)

[https://github.com/mace098/SLHSCENTERSTAGE](https://github.com/mace098/SLHSCENTERSTAGE)

[Old team’s GitHub](https://github.com/orgs/FTC7729/repositories?type=all)

Look at stuff in teamcode for SkyStone

- Box is test robot

Motors, they come with encoders
[https://mindgear.mx/products/neverest-classic-20-gearmotor-am-3102?variant=1188825595931](https://mindgear.mx/products/neverest-classic-20-gearmotor-am-3102?variant=1188825595931)

> Song random guy who came up to us at like the first(?) leadership meeting recomended

violin concerto op 35 Tchaikovsky

Adding a servo (Launch motor)

- For launching the plane

second servo for claw

Make the Auto HW map extend LinearOpMode

```java
public abstract class ChaosAutoHardwareMap extends LinearOpMode {
		// Hardware map here
}
```

## **Robot controls for tele-op**

### Controller 1 — Drive

Left stick Y → forwards/backward

Left stick X → strafe left/right

Right stick X → turn cw/ccw

Right bumper → Run weed wacker

Equations for `driveSpeedA` and `driveSpeedB` taken from [BoxHolonomic](https://github.com/FTC7729/SkyStone/blob/master/TeamCode/src/main/java/org/firstinspires/ftc/teamcode/teleOp/BoxHolonomic.java#L31)

**Holonomic drive**

[Holonomic Drivetrains for FTC series](https://www.youtube.com/playlist?list=PLeUcY-8sTKrP31Lj4mbxPsp_md6CURzd1)

[Holonomic Drivetrains](https://gm0.org/en/latest/docs/common-mechanisms/drivetrains/holonomic.html)

$$
v=\sqrt{x^2+y^2}*sin(\theta+\frac{\pi}{4})
$$

### Controller 2 — Accessories

x and y buttons → control the launch servo

d-pad → control the lift motor

- up = up/deploy

- down = down/reset

a and b buttons → open/close claw

### We need new fuse for battery #8 and #3

# New meeting plans

adding mondays

fridays extended to 6-6:30

Move Fri-15 to Thurs-14

**Build team**

Arm done by break

Design of basket by break - Friday 15th

- 3D print individually during break

Funnel in week after break

**Break**

School is open 18th - 22nd

## **Lessons learned from DCI**


> After our competition at the DC International School, we gathered as a club and discussed how we did and what lessons we learned
> This could probably be good to look back over before another competition

### Things to improve

Need a proper go box

Needed practice before

Spend much more time working on portfolio

Plane is good

Better delegation

We need to write out a script for judging

~~Replace poor quality usb cables~~

Chains

- Chains catching on stuff

- Remove slack from chains

~~Fix directions for strafing~~

Add hanging mechanism to basket

Do more scouting at comps

Place pixel on board and park during auto

We want to hang

Make back up airplanes

Get legal team props?

Create tri-fold

Do more leadership meetings

- and minutes

~~Teach people how to run the robot~~

Move the license plate that is behind the chain

M‌ake pad for control stuff

Fix phones box

### Things we did well

Good points per round

Good attitude when teammates bots had issues

Gracious professionalism

Handling stuff on the fly

Call to remove linear slide

Fixing the binder at the beginning

Write up a checklist to start up the robot

**New basket system**

Still using lifting mechanism

lifting up a bar with the pixel holder on it

Spin the bar around (with a servo) to dispense pixel

---

# Plans for autonomous

If on  far side, move through the gate in the middle to park in backstage

if starting at the back of the field, park in backstage

### **Leadership meeting notes**

**Meeting dates**

long meeting Tuesday

Thursday is also long

Saturday

- Could be as early as 8 ish

- Maybe meet elsewhere to work longer

How are we testing with the backdrop

**Judging for programming**

How build communicated their needs with us

- Needs for safety backups

8 Revolutions all to get all the way up

- the motor is 537.6 pulses per minute 

Continuous control of lift system

- Still needs software endstops

Add d pad left to only close the lift to hanging point

Claw becomes a button that flips and flops it

**Stuff from the middle school**

Allen keys

Phillips screwdriver

Tape measure

## Off season ideas

Build sizing tool

3d Scan bot and 3d print mini bot

3d scan and print Napoleon 

Create “Guide” for next season

- Engineering notebook but just for us

Work on multiple solutions at once

- Design in parallel

- Almost like building stuff for the government/military

  - They want a fighter, everyone makes one, they pick their favorite

- Sorta like competitive

Season starts beginning of August

Herndon Middle school new robotics team

[https://www.chiefdelphi.com/t/what-does-your-team-do-during-the-off-season/128907](https://www.chiefdelphi.com/t/what-does-your-team-do-during-the-off-season/128907)

# Training team

> When we started the offseason, we split up into goofy teams and I was in charge of the training team
> This section consists of goals/plans for what we were going to do during offseason, both as the whole club and as the training team
> Training team was also going to be the brains behind helping with the middle school

Learning Java

Learning onshape cad

Possibly get people a cad or programming certification

- We need to find out how/if we could administer testing for this

Furthering knowledge/skills proficiency with FTC tools (software and hardware)

(hopefully) self led

- Maybe 3 mini teams (one for each pair of phones)

People who want to do CAD/Programming next season

- Maybe we could put CAD with programming under software

  - Encourage a blending between the two groups

Train people to give lessons

- Get them to learn something, they present/teach next meeting

Teaching stuff to middleschoolers, new people who come in with readvertizing, and people already here

**Us**

- Goof off with boxy

  - Use sensors

- Write stuff now

- 2 new freshmen programmers

- **Ideas**
- Andrew teaches wrenches
	- Types of wrenches
	- Types of nuts
	- Types of allen keys
- Andrew unboxing video
- Robot that can be guided using AprilTags
	- Cube with tags on it
	- Top comes towards
	- Bottom goes away
	- Left and right sides strafe
- Build a dedicated servo tester
	- [https://elonics.org/servo-motor-controller-tester-circuit-using-555-ic/](https://elonics.org/servo-motor-controller-tester-circuit-using-555-ic/)
	- Could possibly use minicom to talk to (old) modern robotics servo controllers
		- [https://modernroboticsinc.com/product/core-servo-controller/](https://modernroboticsinc.com/product/core-servo-controller/)
     - Build chassis
     - DIY CNC machine
     - Robot with
     - Build an EV or like vehicle of some sort
     - Mini tesla coil
     - **Robot with arm**
     	- Follows april tag
      	- Tags dictates task
       	- Defensive area
       	- Robot arm
       	- 2 joints
       	- Pick up cube
       	- Pick up and pour cup
       	  - Speed(?) stack?
       - Rotate in two directions
       - Suspend self
       - Put stuff on shelf?
       - Designing as a whole club
       - Possibly make “headless” (relative)
- Tong bot
	- iykyk
- Buy sensors
	- Color sensors - $19 each
		- Probably pretty versatile
	- Touch sensors  - $8 each
		- Kinda mid, could be useful
	- 2m  distance sensors - $29 each
		- Pretty lit 🔥
	- magnetic limit switch - $16 each
		- idk mid I guess
		- Not sure how useful they are
	- **Buying options**
		 - [REV Sensor bundle](https://www.revrobotics.com/rev-45-1885/) - $172.50
   			- 2 x color
   			- 2x touch
   			- 2x 2m distance
   			- 2x magnetic limit switch
   			- 4 pack of red/green indicators
   			- 4 pack of 100mm wires
   			- 4 pack of converter boards
		 - REV Sensor bundle sans converter boards - $157.5
   			- 2 x color
   			- 2x touch
   			- 2x 2m distance
   			- 2x magnetic limit switch
   			- 4 pack of red/green indicators
		 - Our picks - $163.5
   			- 4 x color
   			- 2 x 2m distance
   			- 2 x touch
   			- 4 pack of red/green indicators

**Middle school** 

- Small groups, 2-3
	- lia, lasse from girls team
 	- Techno team is starting from zero

- I want to get them all to try writing actual code, not blocks

  - Python would be great

  - OBJ is actual experience with java

  - Using android studio would be ideal, but I don’t think they can get that 😡

- Teach whole club a little code

  - Get them all exposed

  - They have two teams (these are kinda going away for now), they are building new bots for practice there will be 2 independents groups (~3 people each) learning code at once

- One day a coding challenge for whole team

  - How could this work?

- What programming resources do they have access to?

  - On the robots

    - Mid

  - Has blocks and OBJ editors

  - Tinker CAD??

    - Difficult, requires learning a little electronics

   - ~~Scratch~~

      - ~~Blocked 😭~~

      - Email Mrs Evans with message about scratch

[https://ftcsim.org/](https://ftcsim.org/)

Maybe more advanced for people already in the club

- April tags and computer vision

Create stuff for start of next year to start teaching people again

Make things we can give to sponsors?

- Competition

Daily slides with agenda for each team

- At end say what we did and what we are going to do next meeting

## Timeline

Tues Feb 6 - Work on possible lesson topics

- Methods for how to tech

- Key skills everyone needs

Thurs Feb 8 - Introduced AS to girls

- Copied OBJ code to AS

- It works!

- Overviewed our code

- setting up drive motors and such

- Introduced Git

- They did some debugging on AS

Fri Feb 9

- Recap MS meeting

- Plan for what the hay WE are doing

Tues Feb 13

- HS

   - 2 more programmers

   - Walked them through our TeleOp

   - Learned about robot simulators

- MS 

   - Got started with creating a new OpMode

   - New programmer

Thurs Feb 15

- **Goal:** Create motors in code

   - Have functional on virtual bot or real hardware

   - If real hardware, teach a little wiring

- Counted all the keys on a keyboard

- plus one more programmer

- Learned about where hardware plugs into

- Got through some of the motor setup

Tues Feb 20

- **Goal**: Speedrun the first like 3 weeks of the club in one meeting

   - Get them to upload their own opmode on the phones

- Showed new programmer basic opmode structure and uploaded opmode to robot

- Created basic AprilTag following opmode

- HS

   - We had no computer to program with

   - Got servo motors sorted

- MS

   - I didn't have my laptop

   - They got the rest of the code for motors written

   - Also looked at servos

Fri Feb 23

- Made good version of apriltag following code

Tues Mar 12

- HS

   - Learned about collaboration in using github

- MS

   - Created program to control 2 servos and a motor

   - Added some improvements that should make servo control better

   - Maybe add in checking if either button is pressed

> Okay so yeah i'm not going to mess with the indentation for the code here, this is all yap anyways
> If someone reading this thinks this seems prommising or useful, please pursue this path
> When I was writing this, I thought it had the possibility of being more efficient in some way
> Idea was that reading the movement from the controller could be more costly than storing it all in binary, and parsing that after the fact would save time, maybe?

[Possibly teach them some bitwise stuff](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/op3.html)

```java
01 == //`a` button
10 == //`b` button

if movement > 0:
	direction = 1
	if (n == 2) {direction = -1}
	pos += stepSize * direction
```

What is a bool * double???

Will false = 0 and true = double?

If true, then could do a oneliner. Something like:

```java
movement = (1 * a) + (2 * b) + (4 * x) + (8 * y)

// Might need to convert the bools to numbers by doing something like
a ? 1 : 0
```

Could even add other movement to that

Then the if from before becomes

```java
// let movement = 0b111001

if ((movement & 0b11) > 0){ // equivalent to (((movement >> 0) & 0b11) > 0)
	// movement == 01
} else if (((movement >> 2) & 0b11) > 0) {
	// movement == 10
} else if (((movement >> 4) & 0b11) > 0) {
	// movement == 11
}
```

Full process would look like this

```java
// Init vars
stepSize = something;

// In main loop
movement = (1 * a) + (2 * b) + (4 * x) + (8 * y)

if (((movement >> 0) & 0b11) > 0 ) {
	servo1Position += stepSize * (1 * -((movement >> 1) & 0b1))
}
if (((movement >> 2) & 0b11) > 0 ) {
	servo2Position += stepSize * (1 * -((movement >> 3) & 0b1))
}

//
```

Next time we will have to test 

Friday 15

- Tasks to be completed

- Create the drive motors

- Create the arm motors and servos

- Create basic drive 

   - Forwards/backwards and turn left/right

- Create manual control for arm

April 19

- Profusely apologize for extended leave

- [Review PR](https://github.com/SLHS-Robotics/SLHS-Offseason-2024/pull/14)

- Read Tian’s other PRs and figure out how they should be merged

- Commits for issue 3 did not come through


May 7

- Suggestions from Mr. Davis

   - Instead of teaching programming, teach the concepts

   - Showing them some of what they could do with programming  

Check out ultrasonics for next year

List of approved FCPS tools

[Digital Ecosystem Library  | Fairfax County Public Schools](https://del.fcps.edu/home)

[https://github.com/sethptrend/FtcRobotController](https://github.com/sethptrend/FtcRobotController) MS robotics code

## SL


> Okay so this next section was just what I wrote to submit the time working with the middle school team for service learning for IBCP


My high school’s rookie robotics team uses the most advanced set of tools for programming our robots, and in order to bring in new, knowledgeable team members for next year’s competition season, I volunteered to help teach and tutor students in the Langston Hughes Middle School (LHMS) robotics teams in order to teach them programming and pass on knowledge on the tools that the high school team uses. I joined them at their robotics meetings and worked with them in small groups of three to five students. This year, only three members of the LHMS had proficient knowledge pertaining to programming. The rest of the members of the club, approximately 15 students, had very little to no programming knowledge or experience. I worked to find tools which they could easily access from their school laptops to teach them basic programming knowledge.

Finding appropriate tools was difficult because of various restrictions and criteria I followed when selecting a system. Firstly, the tool needed to be accessible in school and run on their laptops. This immediately limited the selection to web applications, as installing programs to the school computers may be difficult and would be cumbersome for a teaching scenario. As I was limited to web applications, I also needed to make sure that the site I chose would be accessible while connected to the school’s WiFi network. This ruled out MIT’s Scratch, because it is blocked on the school’s network. To keep the process simple, I wanted to use a platform that did not require the students to make an account, as that would be cumbersome. I chose to use OpenProcessing to teach new students because it fit my criteria. OpenProcessing is also designed for creating visuals which could be beneficial as it would be very easy for them to see how their changes effect program execution.

I also worked with them using the advanced programming tools. Our team uses Android Studio to program our robot. I was able to get them access to Android Studio so that they can learn how it works. I was able to teach them how the code is organized in an Android Studio project and the structure for the code that is uploaded to the robot. I was able to teach them all of basic elements that are involved in creating an OpMode for the robot using our tools. 


### MS schedule
> And this was the schedule for the middle school team

Mr. David's planned regular meetings: Regular Hughes Robotics Club meetings: 3/7 6:30-8:30 PM

3/12 6:30-8:30 PM

3/14 6:30-8:30 PM

3/19 6:30-8:30 PM- cancelled

3/21 6:30-8:30 PM - cancelled

3/26 6:30-8:30 PM holiday

3/28 6:30-8:30 PM holiday 4/2

6:30-8:30 PM teacher workday

4/4 6:30-8:30 PM

4/9 6:30-8:30 PM optional (Eid al Fitr begins at sundown)

4/11 6:30-8:30 PM

4/16 6:30-8:30 PM

4/18 6:30-8:30 PM

4/23 6:30-8:30PM optional (second evening of Passover)

4/25 6:30-8:30 PM

4/30 6:30-8:30 PM

5/2 6:30-8:30 PM

5/7 6:30-8:30 PM

5/9 6:30-8:30 PM

5/14 6:30-8:30 PM

5/16 6:30-8:30 PM

5/21 6:30-8:30 PM

5/23 6:30-8:30 PM

5/28 6:30-8:30 PM

5/30 6:30-8:30 PM celebration/party

18 meetings till the end 😭

EOY Party - May 31
