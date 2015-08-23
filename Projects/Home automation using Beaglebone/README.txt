**************************************************************************
                 HOME AUTOMATION USING THE RASPBERRY PI
**************************************************************************

                             INTRODUCTION

The goal of this project will be to create an Internet of Things product
for HOME AUTOMATION using the RASPBERRY PI. This product should allow the
user to monitor his home using a variety of sensors and a camera and also
control some of the appliances in his home such as lights, fans etc. An
easy to use web based interface will be provided for this product so that
the user can customize the functionality.

The key feature of this product is its integration with social media and
online services like Twitter, Facebook, Gmail and Dropbox using their APIs
for real time updates to the user. This makes the process of monitoring
and control easier and more interactive so that a single tweet can be used
to turn on/off the lights and images captured by the camera can be posted
on Facebook or emailed to the user.

**************************************************************************

                        SCOPE OF THE PROJECT

Students undertaking this project will have to create a working product as
described above. It will be up to them to add more features based on their
creativity but there are some minimum requirements that will have to be
met when they attempt this project.

1)  Interfacing Sensors to monitor the home.

	These sensors can be of multiple types. You can choose from a range of
	sensors as long as they will be fully utilized. About 4-5 sensors must
	be intefaced although you may add more if required. Some of the common
	types of sensors are Proximity Sensors, Ultrasonic Range Sensors, PIR
	Sensors and Fire Sensors. Only DIGITAL sensors can be interfaced. You 
	will have to submit a requirement of all the sensors which you plan to
	use (so that they can be ordered for your project).

2)  Interfacing Output devices to be controlled.

	Although this project deals with a lot of hardware interfacing, it is
	not the primary goal. So output devices will be simulated using a few
	LEDs and Buzzers. You are free to choose the type of output devices
	want to interface but you must interface atleast 4-5 sensors. Varied
	types of LEDs can be used.

3) 	Interfacing a USB Webcam.

	A webcam must be interfaced in order to provide video monitoring and
	motion detection features. You may choose to implement any other image
	processing feature using the webcam (as long as it is feasable). Also,
	images that have been captured should be saved on the Pi. This webcam
	will not be provided, so all members will have to contribute towards
	buying one. Any cheap one will do.

4)  BONUS FEATURE - Music player.

	Plug in a pair of speakers and play music over the internet.

NOTE - All peripherals will have to be integrated via social media and
	   other web services.

**************************************************************************

                      WEB INTERFACE AND SOCIAL MEDIA

The WEB INTERFACE must be easy to use and should provide the user to
customize every aspect of the home automation system. This should have
at least the following features although you are free to add more based on
your creativity. The settings should be saved in a database.

1)	Setup I/O devices and Social Media / Web services features.
	
	The interfaces should allow the user to customize the I/O devices that
	are connected to the Pi. This includes adding/removing different
	devices, and being able to select certain preset profiles for devices
	to simplify the process of setting them up. For example, output device
	can be an LED or a buzzer and the user should be able to select the
	type of device so that features such as dimming and glowing the LED
	or making the buzzer beep at set intervals can be enabled. Also you
	can link the input and output devices such that if something is
	triggered, the buzzer will beep etc.

	The user should also be able to setup integration with online features
	by entering login details for the accounts like Twitter, FaceBook,
	Gmail and Dropbox etc. He should also be able to configure the various
	sensors to automatically push updates to social media when they are
	triggered. A similar feature must be implemented for the webcam (with
	motion detection / other image processing algorithm) when it is
	triggered to notify with an email (with the images attached) and save
	the images on Dropbox. Also, simple tweets can be used to control the 
	output devices like "Turn on light 3" and sensor status queries should 
	also be enabled by such a system. Creative use of these online services 
	is encouraged and you will be evaluated accordingly for more features.

	Bonus - Music player : Make an interface for uploading/removing songs
						   It should also be integrated with Twitter.

	Note - Make sure that you include options to enable / disable these
		   features as well. No one likes being flooded by emails / tweets

2)	Monitoring and controlling interfaces.
	
	There should be a simple interface for monitoring the state of all the
	sensors. It should also allow controlling the output devices / music
	player. The specific control functionality of the output devices will
	depend on how it has been configured but the LEDs should have control
	options for brightness and the buzzer should have an option to set the
	beeping frequency and duration with an automatic switch off time out
	setting as well.

	Getting the webcam to work with a live stream will be really cool but
	if it proves too difficult, you should have an alternate interface to
	customize the camera to capture images at regular intervals and then
	display a slide show of the most recent images / allow the user to see
	images taken during a certain time of day.

Note - This web interface will be hosted on the Pi. A nodejs server will be
	   handling all requests. Also, having a good interface is crucial to
	   making this project successful. There's no need for fancy visuals or
	   styling as such but some minimal themes can and should be used. The
	   web interface will consist of substantial coding on both the front
	   and back end so give adequate focus to both parts.

**************************************************************************

                                GUIDELINES

It goes without saying that every part of this project should be coded in
an Object Oriented style. This holds true for both the front and back end
scripts. There are several real world items like I/O devices etc that can
be modelled as objects but do not forget that even more abstract concepts
can be thought of as objects too. You will have to do a thorough analysis
of the different classes that can be created and identify the relationship
between these classes before you write any code. You will also have to
model the different use cases in this project (and there are a lot) and
explain how each of them is going to work and what requirements (both
hardware and software) are key to completing your project.

This analysis will be compiled in the form of a Software Requirements
Specification (there will be guidelines uploaded soon for the same) which
will essentially be like a blueprint for this project. You are advised to
devote plenty of time to this activity since it will be evaluated and it
will make the actual coding part much easier (if you have analysis is
correct). Each member of the team is expected to contribute to all phases
of this project including both the planning and actual implementation in
code. Good communication between team members is essential to completing
this project successfully on time so please divide the work properly and
manage your coordination properly.

When you write code, make sure that you push to GitHub frequently so that
your individual contributions to the project can be tracked easily. Also,
frequent commits will make it easier to rollback to previous versions when
compared to a few massive commits. You are also expected to write code in
a clean fashion, keeping it well organized and modular with proper
documentation for everything. You will also have to write tests for this
project as part of quality assurance. Since this project has a lot of
components, there are multiplr points of failure and testing your code when
it is written will help you identify and eliminate these points of failure.

**************************************************************************

                                FINAL NOTES

This is a really cool project and you will definitely get to learn a lot
while making the home automation system. Your final product will be a
commercial grade product which you can take further if you want. However
you will have to get used to working with the Raspberry Pi and the Linux
Terminal so brush up on that if you have neglected it so far. There are
plenty of Raspberry Pi related resources available online so go and look
at some of them. If you do face issues while setting it up or while trying
to connect to a network or something, let me know. Your focus should be on
the project, not getting the Pi to work, although that part is equally
important. This project is a really large one and is going to take up a
substantial amount of your time so start ASAP. I have attached a few links
for your benefit so that you can get started. I would advise you to make
yourselves familiar with the different APIs (by testing on your laptop).
You can also test the RPi GPIO library on the Pi once it is given to you
but make sure that all the individual components are working before you
start integrating everything together for the project. Best of Luck :)

**************************************************************************

                       IMPORTANT LINKS AND REFERENCES

Javascript Tutorial - https://www.codecademy.com/en/tracks/javascript

HTML / CSS / Javascript Reference - http://www.w3schools.com/

NodeJS Tutorial - http://www.tutorialspoint.com/nodejs/

Please Google for more resources. StackOverflow will be extremely useful
to debug common errors.

GPIO control for input and output - https://www.npmjs.com/package/pi-gpio

Image processing for the Webcam - https://www.npmjs.com/package/opencv

Music player - https://www.npmjs.com/package/node-mplayer

You can use any other libraries if you feel they are better.

Twitter API - https://www.npmjs.com/package/twitter

Facebook API - https://www.npmjs.com/package/facebook-node

Email API - https://www.npmjs.com/package/smtp-connection

DropBox API - https://www.npmjs.com/package/dropbox

**************************************************************************
