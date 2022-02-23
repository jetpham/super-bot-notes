# swerve drive
sources: https://www.youtube.com/watch?v=ykl5CvG53KA, 
modules contain a wheel on pivot
wheels are driven and steered independently of each other
allows simultaneaous translation and rotaion of a robot

## pro
- agility - 2d drive with direction and chasis orientation indipendent
- amazing traction
- tactical stealth - it is harder to read where the robot will move next
- no need for rotational aiming with something like a turret
- different drive modes can be added in software - very flexible
- able to "roll off" off defenders like in soccer 
- very minimal steering hysteresis - very responsive to turning
- robot can be driven with reference to the field orrientation. forward is  the same direction relative to the driver
- very modular and allows easy repairs
- allows more freedom in robot design due to all 4 sides being able to be the leading side. even corners

## Cons
- complexity/ difficulty 
	- it is not easy to exicute and it has ahigh barrier to entry skill wise
	- control software is very difficult compared to tank drive
	- steering backlsh needs to be managed
	- shifting is complex because each module is indipendently driven
- very heavy compared to normal drive train
- cost ~ $1,200 very expensive
- 8 motors are required at the most for 4 modules
- driver training is neccissary and shoudl be orginized
- a bit larger vertically than other drive trains
- time consuming - developing a swerve drive happens over multiple years

## types of swerve drives:
### coaxial
drive and rotation are individually controlled
one motor for each dimention

purchasable, premade designs

### differential
drive and rotation are geared together 
both motors drive the wheels and the difference in the motor's speed determines the wheel rotation

a bit faster than differencial swerves 

much more complex to manufacture and program

most difficult as of recent

## in-wheel
Needs more reserach
originally found in japanese teams in ROBOCON 

## COTS vs Custom:
### Cots:
- no design required 
- expensive
- more difficult to integrate

### Custom:
- needs to be designed
- cheaper
- potentially more compact
- easire to integrate

## importatn design considerations
- motor choice 
- rotating the wheel
- bevel gears
- encoders
- manufacturing

## motor choice

### CIM / MiniCIM:
- tried and tested
- big 
- heavy
- inefficient
- slow to accelrate

### 75pro:
- compact
- lighter
- compareable power
- needs larger reduction
- burns out easily

### NEO / FALCON
- powerful 
- light
-  compact 
- built-in-encoder

#### NEO:
- slightly smaller
- external motor controller
- less power, less current

#### Falcon:
- slightlky larger
- integrated motor controller
- more power, more current
- better integrated encoder
- spline shaft = smaller pinions

## Turning Motor:
200 rpm is good starting point, can go faster depending on motor choice
### BAG / 775pro / RS550:
- tried and tested
- tall
- can be expensive
- can take up space
### NEO / Falcon:
- compact
- standardized parts
- smaller reduction needed
- harder to integrate encoders
### NEO 550:
- compact
- smaller reduction needed
- potentially harder to integrate encoders


## Belts vs Geras vs Chain:
Continuously variable transmission is good
### Belts:
- least backlash
- least likely to slip
- lightest
### Gears:
- Some backlash
- simple
- potentiall heavy
### Chain:
- most backlash
- can slip and stretch
- heaviest

## Bevel gear setups:
this section applys only to coaxial swerve drive setups
### bevel beside wheel:
- bevel gear is on the same shaft as the wheel
- usually has a non - 1:1 reduction
- more compact
- more expensive
- more complex
### additional gear reduction:
- uses a set of miter gears and additional reduction
- cheaper, easier to procure
	- bevel gears can be bought off VEX
- simpler
- much less compact

## Supporting the drive shaft:
### Bushing:
- metal hub rotates inside a plastic bushing
- durable
- cheaper
- much less compact
### bearing:
- large thrust bearing
- durable
- more expensive
- much more compact

## encoders
necessary to control the drive
### truning encoder
- should be geared 1:1 with module rotation to make it simple to code
- use an absolute encoder
	- absolute encoders remember their zero position
	- incremental encodersr reset their zero position after a power reset
- Good options
	- CTRE mag, US digital MA3 encoder
	- Lamprey Hollow bore encoder
## manufacturing
- cut down on manufacturing time wherver possible
- Manufactuable > robust > light
- minimize unique parts
- COTS parts good (if possible and usable)
- 3d print where possible, saves weight and manufacturing time

