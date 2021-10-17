👶 Creation | 🛠 Applications/Use cases | 👍 Pros | 👎 Cons

<img src="https://docs.unity3d.com/uploads/Main/MecanimHowItFitsTogether.jpg" width="600" height="280">

### Animation clip
> A _**single linear recording**_ containing information of _**changes in properties over time**_ (position, rotation, etc) of a certain object
+ 👶 Creation: in Unity, humanoid motion capture, in external 3D application, Unity asset, timeline 
+ Examples: "Walk", "Idle", etc

### Keyframe
> Each point on clip containing information of _**properties at a specific time**_ of a certain object 

### Animation curve
> Attached to _**[animation clip](#animation-clip)**_ to indicate _**how (smoothness/roughness) a property change**_ from one _**[keyframe](#keyframe)**_ to another

### Automatic keyframing
> In Animation mode, any changes applied to an object from _**Scene view**_ or _**Inspector**_ will be _**recorded**_ as _**[keyframes](#keyframe)**_

### Playhead
> The _**while line**_ in Animation Timeline indicating where to add a _**[keyframe](#keyframe)**_

<img src="https://connect-prd-cdn.unity.com/20210123/learn/images/11f918b1-464c-407e-9d0c-f2fd5e67d752_image10.png.2000x0x1.png" width="600" height="200">


### Animation curve

### Avatar

### Avatar mask

### Humandnoid animation retargeting
> Apply the _**same set of animations**_ for various _**humanoid models**_ utilizing _**[avatar](#avatar)**_

### Animation event

### Animator controller

### Animator component
> _**Assign animation**_ to a GameObject, require a reference to an _**[animator controller](#animator-controller)**_ and an _**[avatar](#avatar)**_ (if the GameObject is a humanoid character)

### Root motion	
> Allow animation to _**change the position and rotation according to the uppermost parent**_ of the GameObject (# w/o root motion: according to the world coordinate)
+ Example: object with initial Y=0, animation Y-1 then Y+2. W/ root motion, Y=1 (-1+2) after 1st animation, 2nd animation starts from Y=1, Y=2 after 2nd animation... W/o root motion, 2nd animation starts from initial Y=0, so do 3rd/4th...

### Culling mode
> Decide whether to animate while the GameObject is off-screen (not renderred)

### State machine

### Mecanim
