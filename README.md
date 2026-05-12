# BLINKYYY_BOARDD
This project is based on the stasis guide on the blinky board, where I mostly followed the guide and changed the final look of the PCB to be a FISH (a FIH if you may):

The circuit is based on the original LED chaser design using a 555 timer IC and a CD4017 decade counter. The LEDs light up sequentially, creating a moving animation around the fish-shaped board. While the electronics stay close to the original tutorial, most of the work went into redesigning the PCB layout and making the board look unique.

# Process

The project, first of all, went through the schematic stage as all projects do. It wasn't anything too interesting. For this project ill be using KiCad.  The guide used a 555 chaser and a 4017 IC, which sounds like random letters and words, but kinda makes sense if you think about it. For example, the 555 timer in this build is kinda the "brain" of the whole build, and as far as I understand, the name comes from the 3x 5K ohm internal resistance, while for the IC unit it would help me connect 10 LED's to the board with ease because it has so many pins (think of it as a "spreader" here). Other than those 2 parts, the other parts in the kit are really simple, like an LED, resistors, a polarized (+ and - differentiate in this one, so be careful when wiring!), and a normal capacitor (don't forget the potentiometer too!!).

After understanding what everything dose the next step was to wire all of them, which wasn't difficult at all, except for the wiring for the 555 timer. For context, the timer has 3 modes:
- Monostable (for time delays) mode, which is usually used as a stopwatch
- Astable Mode, which shifts between high and low
- Bistable Mode, which is like a toggle mode (eg a LED turning on and off with different buttons)
For my build, I followed the Astable mode, which has a bit of a weird wiring, but it wasn't too hard.
Also, usually when routing, I learnt it's better to label wires (by pressing A) so it's easier to understand than to wire everything in one fell swoop.
After all of that, the schematic looks a bit like this:

<img width="977" height="603" alt="schematic_photo" src="https://github.com/user-attachments/assets/407fd724-5712-4191-b89d-09e496c90a9e" />

# The PCB 

Finally, were are onto the PCB designing. Before this, of course you first had to add footprints, obviously. Don't know what they are thinking of symbols and footprints like this, imagine a symbol, something used to understand how a part has to be routed, it's for our case, the symbols are the 555 timer, the IC... everything on the schematic that counts as a part is, and as for footprints Its how the part would look like on the real pcb itself. So I mostly did the same footprints assigning like on the guide this:(+ you will have to download the footprint from [sign in and download](https://app.ultralibrarian.com/details/15b11d40-103f-11e9-ab3a-0a3560a4cccc/Texas-Instruments/CD4017BE]) )

<img width="1063" height="466" alt="b4llal" src="https://github.com/user-attachments/assets/b1f1c9fa-1b88-4eac-96af-b68b95fdaa06" />

After that, open the PCB designing on KiCad and press F8 or just click update PCB from schematic,  and boom, you're almost done. The next logical step would be to make your own design and place parts and finally route everything, and you're finished (sounds like a lot, but  it's actually not that difficult)
In the PCB, I changed the whole look of it by changing the Edge.Cuts (which are like where the PCB must be cut to get that shape) using the tools on the bottom and middle right. For me, it was in the shape of a Fish...
One of the most interesting parts of this project was adapting the circuit into a non-standard shape. Since the board outline was no longer rectangular, component placement and routing became much more challenging. I had to carefully position LEDs and traces so the board still looked clean while maintaining proper electrical connections.
Finishing off, you usually place the parts on the PCB and route it by placing traces of copper to connect the parts highlighted.

## Tools Used
- KiCad
- GitHub
- JLCPCB
- Hack Club Stasis Guide

## Preview
Here's the final look of the project:
(At the end, I added an extra IC to connect more LED's to make the spiral blinking look cooler and smoother)
<img width="910" height="492" alt="schematic_photo(final)" src="https://github.com/user-attachments/assets/81c4cf2d-f5de-481e-a4c1-9400528e0bb6" />
<img width="771" height="526" alt="PCB(2d)" src="https://github.com/user-attachments/assets/cc05fbfa-63d0-4b2d-9309-9071a16cf107" />
<img width="1150" height="618" alt="PCB(3d)" src="https://github.com/user-attachments/assets/6a33650b-cafe-42f8-a1e8-01d194463ff0" />

## Credits
Original guide and inspiration:
- Hack Club Stasis
- Hack Club Blueprint

Guide used:
https://stasis.hackclub.com/starter-projects/blinky

## Conclusion
Overall this is a perfect project for a begginer to start getting into making these cool custom PCB's and, I really recommend people who start getting into this type of hobby to start from a reallyy easy project like this!Big thanks to [Hack Club Stasis](https://stasis.hackclub.com/starter-projects/blinky?utm_source=chatgpt.com) for the awesome beginner-friendly PCB guide that helped me learn PCB design and customization.
