# Theremin

## Introduction:
Imagine making music by just waving your hand in the air, as if you are conjuring melodies from the air itself. That's the magic of the Theremin!. Invented in the 1920s, this electronic marvel produces ethereal sounds without sounds.

The theremin operates through capacitance sensing and frequency mixing, comprising of pitch and volume circuits. The pitch and amplitude oscillator emit continuous electromagnetic fields altering the frequency and amplitude as the player's hand near the pitch antenna, generating higher pitches closer and lower ones farther away, the amplitude also changes depending on the distance of the player's hand from the amplitude antenna by taking advantage of the parasitic capacitance of the human body.

![WhatsApp Image 2024-05-11 at 19 21 01_c787b093](https://github.com/Projects23-24/Theremin/assets/133627261/73382de1-57e6-4771-8310-ac378054b968)

## Methodology:
### Frequency Block:
A high frequency Colpittis Oscillator of 400KHz built using LM358 opamp was used to detect the change in capacitance of the tank circuit by taking advantage of the parasitic capacitance of humans. The antenna acts as the first plate and the player's hand as the second, hence by changing the distance of the player's hand from the antenna, he changes the effective capacitance of the Colpitts oscillator tank circuit. It is designed to change its frequency by not more than 20KHz.

Now by mixing this signal with a sine wave of frequency same as that of the tank circuit (without the player's hand). We extracted two waves of frequencies. The first one has a frequency equal to the sum of the frequencies of the two signals and the second one has its frequency equal to the difference between the frequencies of the two signals. The lower frequency wave can be extracted by just passing the signals through a low pass filter. It is to be noted that this obtained wave has a frequency less than 20Khz (Since the Oscillator is designed to not change more than 20KHz) and hence in audible range. 

### Amplitude Block:
Now we mirror the frequency block and connect its output to a Butterworth Salen Key low pass filter (A second order, active filter ) with a very low cut-off frequency so that the frequencies of audible range lie on the transition band. Since the frequencies lie on the rapidly falling slope of the graph, each frequency will be associated with a specific DC gain (or I guess attenuation would be a better word). Now that we assigned a voltage to a frequency we integrated it with a Voltage Controlled Amplifier . Hence now we control the gain by varying the player's hand's distance from the antenna.


### Project Veterans:
1) VENU MADHAV P L
2) VASANTHAKUMARAN
3) HARDIK JAIN

##### Lets connect and have a Chat!💬
<a href="https://www.instagram.com/electronicsclubiitg/?hl=en" ><img src="https://upload.wikimedia.org/wikipedia/commons/a/a5/Instagram_icon.png" width="45" height="45"></a>
<a href="https://www.facebook.com/electronics.iitg/"><img src="https://1000logos.net/wp-content/uploads/2021/04/Facebook-logo.png" width="78" height="50"></a>
<a href="https://www.reddit.com/r/ElectronicsClubIITG/"><img src="https://www.pngkit.com/png/full/0-7757_reddit-logo-reddit-icon-png.png" width="45" height="45"></a>
