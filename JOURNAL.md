# Day One 18/05/2026 8.5 Hours
## Background
Okay third times the charm.

This project is my third attempt at making a cyberdeck, between lots of new inspo (Mainly [This](https://youtu.be/gIWp_F9PPzI?si=jBwlFPpAz0U6D1uZ) video) and ideas along with not liking my other builds I decided to make this one. The whole goal of this build is to be robust, modular, and work off grid. For that I'm using a rail system that allows you to swap out different peripherals as you see fit, for now this includes a battery and meshtastic relay. The goal of the meshtastic is to allow you to easily communicate with other people while out of cell range. Additionally the RETAKM will work to control manufacturing systems and view/develop CAD models.
## Work Done
Thanks to my now quite large amount of time making objects like this I was able to get a whole lot done in a day. I started by figuring out the max size I needed the case to be. The largest part I had to fit was 100% the screen, being a 10.5 in display, the same one from my last cyberdeck build. I gave ample space on each side for cable routing and stuff then got to work on the bottom shell now that I knew what size the case had to be.

<img width="1147" height="883" alt="image" src="https://github.com/user-attachments/assets/0a02b63b-e311-4e7e-a681-30d482397846" />

For the bottom of the case I needed to fit a keyboard and Pi. At first i also was thinking of having the meshtastic intergrated but I feel being able to swap the mesh hardware out would be a good feature so i decided against it afterwards. A annoying thing I had to figure out with the bottom was how to mount the keyboard without any holes in it, I also didn't plan well for cable routing at first. To fix the keyboard mount I made a retaining piece that screws into the rest of the bottom shell.

<img width="1182" height="370" alt="image" src="https://github.com/user-attachments/assets/9e000163-29ca-4a37-b104-156cdb103a4a" />

Next I learned how to import other CAD models so that I could have a Pi referance. Usining the Pi referance I made a standoff mount to allow the power cable to be routed under the Pi. I also had to mount the keyboards data line as it was seperate from the rest of the PCB.

<img width="919" height="667" alt="image" src="https://github.com/user-attachments/assets/bacc327c-d92f-49c7-9267-4d766f89f492" />

After making the bottom mount I went on to work on the screen mount. The screen mount is extremly simple, making use of the VESA on the back of the screen. The hard part is sliding and pivoting the screen off of the bottom to expose the keyboard. To handle that I'm employing the help of my partner Evan who is going to help with CAD a small bit so I can learn more, but a ton with electrical and software related to the build.

<img width="1582" height="979" alt="image" src="https://github.com/user-attachments/assets/de3cf999-7bab-4cf1-936f-6adb59141738" />

## Tomorrows goals are:
- Have Evan make the slider
- Mount the peripheral rails
- Figure out the external battery system 

# Day Two 19/05/2026 2 Hours

Okay today had a large pivot in the design idea. Evan looked at the build and realized that a lot of things were not really optimized. The big problem was the screen, the original design used a portable monitor which was both bulky and expensive, they suggested to switch to a IPS panel to cut down on cost while allowing for a larger screen but smaller footprint. They landed on this screen https://www.aliexpress.us/item/3256801507917524.html Additionally they realized that the keyboard mount was pretty unoptimized so I'll need to make a actual model of the PCB to make a better mount for it. Fixing both of those _should_ let us shrink fown the footprint a fairly large amount while giving us a larger screen. The only downside of this being no speakers built in. To fix that at some later point I'll look into making a module that mounts to the back with a speaker in it.

## New Goals:
- Make Keyboard PCB
- Fix Screen Mount
- Add rails

# Day Three 20/05/2026 Hours 3

Okay today Evan got to work on the screen mount redesign. This meant adding in the new screen and making a mock up off it for the CAD, I also made a mock up of the keyboard PCB so we can make sure the size fits well. Lots off time today was spent trying to figure out how to make sure the screen can both pivot and slide forward and backwards. The design we settled on makes use of a clamping lock for the hinge similar to a bike. 

<img width="443" height="444" alt="image" src="https://github.com/user-attachments/assets/34601461-4139-4936-9c1b-2279fd8beb7c" />
<img width="1399" height="839" alt="image" src="https://github.com/user-attachments/assets/16bdcbee-e50c-425d-afd8-7f4912d373bc" />

This is nice because it's cheap while remaining robust and leaving ample room unlike the original idea of using a ratcheding door hinge.

For the slide we decided to keep things simple and familer and we went with MGN7 rails, they're fairly cost effective and still strong enough for what we needed. Thanks to a miscommunication Evan actually improved the design and made it so that you can have the screen in three different "modes". A tablet mode where the hinge is at the bottom of the rails and only has the screen visable, a laptop mode where you slide the screen up and tilt the hinge slightly to access the keyboard, and a closed mode where the hinge is at the top of the rails and allows you to close the lid with the screen internal.

<img width="447" height="355" alt="image" src="https://github.com/user-attachments/assets/506389d3-aa11-4e91-afca-e22cd9cd30ab" />

**Screen**

<img width="1535" height="994" alt="image" src="https://github.com/user-attachments/assets/7c636260-9f74-4584-842f-d7c4fc564df8" />

## Tomorrows goals are:
- Idk I seem to be really bad at goal setting
- Make the damn battery

# Day 4 21/05/2026 Hours 3

We pivot again.

Realized that the new screen was gonna be a lot more effort than it was worth so I decided to switch back to the old one. Also got the keyboard model placed into the RETAKM model and got some tolerances fixed for it. 

<img width="1606" height="1101" alt="image" src="https://github.com/user-attachments/assets/a1ee5e9d-a5a9-43fd-8126-0840a7246256" />

Next I got all of the mounts figured out for the IO ports. We went with G16x4 ports as they're very durable but still are able to do usb signal for cheap. They also just look cool, my only worry is that they may hit the keyboard power PCB.

<img width="1556" height="936" alt="image" src="https://github.com/user-attachments/assets/ffabd825-d776-49a0-b268-85aae18ddff4" />

Last I found a dope [model](https://www.printables.com/model/424732-ryobi-battery-adapter-usb-powerbank-version) that @donutcat already made that I can modify to work as a battery for the Cyberdeck.

<img width="1482" height="994" alt="image" src="https://github.com/user-attachments/assets/a117da62-5937-4f87-befb-8828a273d760" />

Pretty proud of the amount of work that's been done in such a short amount of time.

## Tommors goals are:
- Install the slider system
- Work more on the battery
