# hxsMidiSwitcher
Simple 8 button MIDI controller for Line 6 HX Stomp using Nano clone

I'd originally shared this at https://www.basschat.co.uk/topic/338238-build-your-own-midi-controller-i-did/ but it's been pointed out (Thanks Josh!) that this would be a more sensible place for it.

It works OK and has served me fairly well over the last ~8 months I've been using it, but v2 is in the works with a touchscreen and expression pedal input...

Basic description (from that thread - although there's more info there if you want to trawl through the entire thread...

I wanted to add some more control options to my Stomp and was looking at controllers like the Morningstar MC6, but couldn't justify the £200 outlay.. so looked into making one myself - and it's turned out to be far easier and cheaper than I expected.

Total cost for all the electronics and switches is about £25 -30 depending on how confident you are at slightly fiddly soldering... the extra few quid gets you a pre-soldered microcontroller and an adaptor board with screw terminals, so the only soldering you'd need to do is for the wires to the tags on the footswitches and on the MIDI socket.

And then you'll need something to house it in. I made a 3d printed enclosure for mine, but any box you can buy/build/modify will do.

If anyone's interested in making something similar for themselves, I'd be happy to share wiring diagrams and the code I used. I'm no electronic engineer or programmer, so no doubt there's plenty of room for improvement, but I've got it to work well enough to do what I need it to, and maybe it'll work for you too? I'm happy to help with tweaking it for slightly different configurations if you'd want a different layout.

What it does:

You press a footswitch, and it sends a MIDI message. The way I have mine setup is that it either sends a MIDI PC (Program Change) message to change preset patch on my HX stomp, or a MIDI CC (Control Change) message to change any of a number of other settings or parameters. It could potentially send MIDI notes as well if you wanted to use it as a pedal keyboard to play a synth with, I suppose.

If you hold a footswitch down, it can send a different MIDI message (I only use this for activating the tuner by holding the tap tempo button so far, but it could be setup for any of the switches)

If you press more than one footswitch down at once, it can do something else again depending on which ones you press. Mine is set so that pressing 1+2 or 2+3 switches through different pages / banks of button configurations, and pressing 7 + 8 is a sort of panic mode which resets the HX stomp to preset 1, and resets the controller back to the first page.

What it can't do:

It's not programmable from the unit. To change the way the buttons are configured you need to tweak the code and then re-upload it. There's probably a more elegant way to deal with this, but it works well enough for me as is - I don't expect to need to reconfigure it very often once I've got it set up.

Right - I'm gonna stop there for now.... if no-one's interested then I'm just rambling into the void for nowt. If anyone is interested though, let us know and I can post more details. Or, if you know more than me and can spot where I've gone wrong or what I should have done better - lemme know and I'll try and improve it!

 

Cheers,

 

stoo
