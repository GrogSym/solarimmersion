# solarimmersion
excess solar to hot water tank via home assistant

It should go without saying that mains voltage is dangerous, and this should only be attempted if you are competent and comfortable that you can deal safely with electricity.

I have included a parts list

The ESP32 board is connected to the SCR via 3 of the 4 available pins on the SCR that connect to the screen (the screen is not used in the project). The 5v can be ommitted, as the ESP will get power from the HiLink. The dallas board is also connected to the ESP32.

The mains power coming in goes to the 'in' for the Sonoff (this is also where I've taken power for the HiLink). The output goes to the SCR 'in'. The SCR 'out' then goes to the hot water tank immersion. 

I have also included a mechanical timer on my set up as I heat the water tank via cheap rate electricity over night. The SCR board is not 100% efficient as it generates heat, so is not ideal for that use.

One further note, CT clamps do not work with SCRs (which I found out the har way), hence the sonoff.
