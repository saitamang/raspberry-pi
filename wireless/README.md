# Wireless Testing

SUMMARY:

Car control hijacking: rolljam attack

- install radio frequency transmitter for Raspberry Pi(rpitx)
- On the PI have an RTL device connected for receiving and a piece of wire connected to GPIO4 (pin 7)
- You can solder one on or if it has soldered pins already use a jumper wire and cut off the other end or something
- then on laptop install the frequency reader (gqrx). Connect the RTL-SDR to your linux machine. Run the GQRX tools and set your frequency to read. 
- The key fobs for malaysian cars tend to be around 433.9Mhz so monitor that, get another RTL for your laptop so you can monitor what's happening
- You can just use ./rtl-menu.sh for most of the work, set both receive and transmitting frequencies to 433.9Mhz
- Press record and then use the key fob's unlock button (make sure you're far away from the car itself before you do this)
- Then go back and select Transmit and should work if your car uses a similar system to the car


## RTL-SDR ##

<img src="https://cdn-learn.adafruit.com/assets/assets/000/020/041/medium800/raspberry_pi_DSC00706.jpg" width="400" height="300" />

Basically what I am doing is by reading the frequency transmitted by another transmitter from my pi.

1. Install the frequency reader into your machine

`http://gqrx.dk/`

#This is for laptop linux machine

<img src="https://farm9.staticflickr.com/8603/30105972096_5447126eb2_c.jpg" width="400" height="300" />

2. Connect the RTL-SDR to your linux machine

3. Run the GQRX tools and set your frequency to read

#Noted that the frequency is in KHz instead of MHz

4. Then I am installing rpitx from below link

`https://github.com/F5OEO/rpitx`

#Make sure this one if from your PI, kindly read the repo from given link

5. Set the frequency to test

Example used in video:
- 434 MHz
- 313 MHz

Thank you!
