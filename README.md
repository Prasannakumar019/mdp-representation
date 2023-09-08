# MDP REPRESENTATION
# AIM:
To represent any one real-world problem in MDP form.

# Problem Description:
Consider an AI agent optimizing elevator operation in a high-rise building to efficiently transport passengers between floors.

# State Space:
state_space = {

    "Elevator1": 0,  
    
    "Elevator2": 1,
    
    "Elevator3": 2,  
    
    "PassengerWaiting": 3  

}
# Sample State:
sample_state = "Elevator1 -> 5"

# Action Space:
action_space = {
    "MoveUp": 0,  

    "MoveDown": 1,
  
    "OpenDoors": 2,
  
    "CloseDoors": 3  

}

# Sample Action:
sample_action = "MoveUp -> 0"  

# Reward Function:
reward_function = {
    "PassengerServed": +1,  

    "EfficientOperation": +0.5,  

    "EmptyTrips": -0.5  

}

# Graphical Representation:
![WhatsApp Image 2023-09-08 at 21 20 56](https://github.com/Prasannakumar019/mdp-representation/assets/75235090/674d8321-2b44-44f2-924e-df4ae4d95fd1)


# Python Dictionary Representation:
```
P = {
    0: {
        0: [(0.9, 0, 1, False), (0.1, 1, 0, False)],
        1: [(0.1, 0, 1, False), (0.9, 1, 0, False)],
        2: [(0.0, 0, 0, True)],
        3: [(0.0, 0, 0, True)]
    },
    1: {
        0: [(0.1, 0, 1, False), (0.9, 2, 0, False)],
        1: [(0.9, 0, 1, False), (0.1, 2, 0, False)],
        2: [(0.0, 1, 0, True)],
        3: [(0.0, 1, 0, True)]
    },
```
# Output:
<img width="604" alt="pic" src="https://github.com/Prasannakumar019/mdp-representation/assets/75235090/edd04726-c826-461b-9a9e-1557a358dabd">

# Result:
Thus the given real world problem is successfully represented in a MDP form .
