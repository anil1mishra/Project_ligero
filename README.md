The application provides a graphical interface for controlling various electrical appliances.
It detects presence in a room and operate appliances accordingly.
It calculates units of electricity consumed by each appliance.
It sets schedule various devices to switch on/off automatically.

Structure of the Model
Two sets of laser sensors and detectors are installed on either sides of the door. This is use to detect movement inside or outside of the room. The signal of the detectors is sent to a microcontroller which is responsible for carrying out all operations. A relay module is connected to the microcontroller and the appliances which are to be controlled are connected to the relay. The microcontroller sends signals to the relay which is used to change the state of the appliances accordingly.

Automatic Room Light Controller with a Visitor Counter
This system is designed by using two sets of Laser transmitters (KY008) and LDR receivers. These sensors are placed in such a way that they detect a person entering and leaving the room to turn the home appliances. In this system, a microcontroller is the central processing unit of this project which is of BCM2837 controller from the Broadcom family. This system facilitates a bidirectional visitor counter for displaying the number of persons inside the room.
When no people are present inside the room, by default all lights will be switched off. When there is movement detected inside the room by the visitor counter, the lights turn on automatically.

Light Control Through Mobile App The app allows the user to manually control the appliances. The user can also set a schedule for automatic operation of appliances. The changes made on the app are updated on the database and the microcontroller fetches the updated values to complete the desired operation. The app also shows the units of electricity consumed by each appliance thereby calculating the total electricity bill which helps to monitor the usage.
The authentication feature adds a layer of security to the system and ensures that no unwanted person accesses the network.

An extension to this idea is implemented in large size room where a room is divided into regions and each region has a particular set of appliances. When there is presence detected in that region, the appliances will switch on. A common example where such situation arises is a classroom when only half of the room is occupied but all the appliances are switched on. Using this, only the required ones will be on.
Here, one laser represents one region. When no one is present in region 2 and only the 1st region is populated with people, only the appliances corresponding to that region with switch on. If people are present in all the regions, all the appliances will turn on.

The 2 LDRs are connected to the GPIO pin numbers 17 and 27 of the Raspberry Pi 3B and the two lights which are controlled are connected to the GPIO pin numbers 20 and 26.

Link to working of the prototype: https://www.youtube.com/watch?v=8sECTSnM5aU
