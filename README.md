# Dance-Off
GoPiGo3 dancing code for autonomous control project

def _gopigo3_command_dance_off(self):
        beat = 60/121
        
        self.gopigo3.set_speed(1000)
        self.gopigo3.right()
        sleep(beat*0.2)
        self.gopigo3.steer(30,100) #line 1.
        sleep(beat*4)
        self.gopigo3.steer(100,25) #line 2.
        sleep(beat*8) 
        self.gopigo3.stop()
        sleep(beat*1.3)
        self.gopigo3.backward() #line 3.
        sleep(beat*0.4)
        self.gopigo3.forward()
        sleep(beat*0.3)
        self.gopigo3.stop() #third boom & line 4
        sleep(beat*0.5)
        self.gopigo3.backward()
        sleep(beat*0.4)
        self.gopigo3.stop() #fifth boom & wait
        sleep(beat*2.4)
        self.gopigo3.forward() #line 3.5
        sleep(beat*0.4)
        self.gopigo3.stop()
        sleep(beat*0.4)
        self.gopigo3.backward()
        sleep(beat*0.4)
        self.gopigo3.forward()
        sleep(beat*0.4)
        self.gopigo3.turn_degrees(-45) #line 6.
        sleep(beat*0.4)
        self.gopigo3.forward()
        sleep(beat*3.6)
        self.gopigo3.set_speed(300)
        self.gopigo3.right() #line 7.
        sleep(beat*4)
        self.gopigo3.set_speed(1000) 
        self.gopigo3.forward() #line 8.
        sleep(beat*4) 
        self.gopigo3.set_speed(290) 
        self.gopigo3.left() #line 6. alteration 
        sleep(beat*3)
        self.gopigo3.set_speed(1000) 
        self.gopigo3.turn_degrees(-15) #line 9. 
        sleep(beat*0.2) 
        self.gopigo3.forward() 
        sleep(beat*3.3)
        self.gopigo3.steer(20,100) #line 1. alteration
        sleep(beat*4)
        self.gopigo3.forward() #line 8. alteration
        sleep(beat*2.2) 
        
        x = 0
        while x < 2:
            self.gopigo3.left() #line 10.
            sleep(beat*0.6)
            self.gopigo3.right()
            sleep(beat*0.6)
            x = x + 1
        
        self.gopigo3.stop()
        sleep(beat*4) #line 11.
        self.gopigo3.set_speed(500)
        self.gopigo3.turn_degrees(-15) #line 9. alteration
        sleep(beat*0.2) 
        self.gopigo3.forward() 
        sleep(beat*3.4)
        self.gopigo3.backward()
        sleep(beat*3.4)
        self.gopigo3.left() #line 6. alteration 
        sleep(beat*2)
        self.gopigo3.forward()
        sleep(beat*2)
        self.gopigo3.right() #line 12.  
        sleep(beat*2)
        self.gopigo3.forward()
        sleep(beat*2)
        self.gopigo3.backward() #line 13.  
        sleep(beat*3)
        self.gopigo3.left() #line 14. alteration
        sleep(beat*1.5)
        self.gopigo3.backward()
        sleep(beat*2.5)
        self.gopigo3.right()
        sleep(beat*1.2)
           
        x = 0
        while x < 2:
            self.gopigo3.turn_degrees(40) #line 15.
            sleep(beat*0.3) 
            self.gopigo3.backward()
            sleep(beat*0.4)
            self.gopigo3.forward() #line 8. alteration
            sleep(beat*0.4)
            self.gopigo3.turn_degrees(-40) #line 16.
            sleep(beat*0.3) 
            self.gopigo3.backward()
            sleep(beat*0.4)
            self.gopigo3.forward() #line 8. alteration
            sleep(beat*0.4)
            x = x + 1
        self.gopigo3.right() #line 7.
        sleep(beat*4)
        self.gopigo3.left() #line 17.
        sleep(beat*4)
        
        x = 0
        while x < 2:
            self.gopigo3.turn_degrees(40) #line 15.
            sleep(beat*0.3) 
            self.gopigo3.backward()
            sleep(beat*0.4)
            self.gopigo3.forward() #line 8. alteration
            sleep(beat*0.4)
            self.gopigo3.turn_degrees(-40) #line 16.
            sleep(beat*0.3) 
            self.gopigo3.backward()
            sleep(beat*0.4)
            self.gopigo3.forward() #line 8. alteration
            sleep(beat*0.4)
            x = x + 1
        self.gopigo3.right() #line 7.
        sleep(beat*4)
        self.gopigo3.left() #line 17.
        sleep(beat*4)
        self.gopigo3.stop() #line 4. alteration
        sleep(beat*8)
        self.gopigo3.forward()
        sleep(beat*4)
        self.gopigo3.forward() #line 8. 
        sleep(beat*4)
        self.gopigo3.backward() 
        sleep(beat*4)
        self.gopigo3.forward() #line 8. 
        sleep(beat*8)
        x = 0
        while x < 6:
            self.gopigo3.left() #line 18.
            sleep(beat*1)
            self.gopigo3.right()
            sleep(beat*1)
            x = x + 1
        self.gopigo3.stop()
