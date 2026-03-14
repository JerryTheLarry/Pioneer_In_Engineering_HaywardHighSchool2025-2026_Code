# Bot_1 Code
Wheel_motor = "6_6925048702386060390"
Arm_motor = "6_14481984369978712988"


def autonomous():
    Robot.set_value(Wheel_motor, "velocity_a", 1)
    Robot.set_value(Wheel_motor, "velocity_b", -1)
    Robot.sleep(10)
    
    
    
    pass

def teleop():
    while 0 == 0: #set a loop
        # Wheels movement 
#        if (Gamepad.get_value("joystick_left_y") >= 0.1 or Gamepad.get_value("joystick_left_x") >= 0.1) or (Gamepad.get_value("joystick_left_y") =< -0.1 or Gamepad.get_value("joystick_left_x") =< -0.1):
#            Robot.set_value(Wheel_motor, "velocity_a", Gamepad.get_value("joystick_left_y")+ Gamepad.get_value("joystick_left_x"))
#            Robot.set_value(Wheel_motor, "velocity_b", -(Gamepad.get_value("joystick_left_y")- Gamepad.get_value("joystick_left_x")))
       
       

        
        if Gamepad.get_value("dpad_up"): 
            Robot.set_value(Wheel_motor, "velocity_a", 0.02)
            Robot.set_value(Wheel_motor, "velocity_b", -0.02)
            
        elif Gamepad.get_value("dpad_down"): 
            Robot.set_value(Wheel_motor, "velocity_a", -0.04)
            Robot.set_value(Wheel_motor, "velocity_b", 0.02)

        elif Gamepad.get_value("dpad_left"):
            Robot.set_value(Wheel_motor, "velocity_a", 0.02)
            Robot.set_value(Wheel_motor, "velocity_b", 0.02)
        
        elif Gamepad.get_value("dpad_right"):
            Robot.set_value(Wheel_motor, "velocity_a", -0.02)
            Robot.set_value(Wheel_motor, "velocity_b", -0.02)
        else: 
            Robot.set_value(Wheel_motor, "velocity_a", 0)
            Robot.set_value(Wheel_motor, "velocity_b", 0)
    
        # Hand Movement
        # Y button move hand up; A button move hand down
        if Gamepad.get_value("button_y"):
            Robot.set_value(Arm_motor, "velocity_a", -1)
    
        elif Gamepad.get_value("button_a"):
            Robot.set_value(Arm_motor, "velocity_a", 1)
        
        # Scoop Movement
        # Right bumper scoop things in; Right Trigger scoop things out 
        elif Gamepad.get_value("r_bumper"):
            Robot.set_value(Arm_motor, "velocity_b", -0.25)
    
        elif Gamepad.get_value("r_trigger"):
            Robot.set_value(Arm_motor, "velocity_b", 0.25)
        else:
            Robot.set_value(Arm_motor, "velocity_a", 0)
            Robot.set_value(Arm_motor, "velocity_b", 0)
def autonomous_actions():
    pass
