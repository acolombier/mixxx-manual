# Example Setups

This chapter presents some example hardware setups with instructions for how to configure Mixxx to work with them.

## See Also

* [Hardware](hardware.rst): background information about different types of equipment.
* [Getting Started with Sound I/O](getting_started.rst): details about each available input and output option.
* [Microphones](microphones.rst): details for configuring Mixxx to work with microphones.
* [DJ Hardware Guide](https://github.com/mixxxdj/mixxx/wiki/Hardware-Compatibility): lists specific devices with information about their prices, features, and compatibility with Mixxx.

## Computer Only

The built-in audio interface on most computers comes with a single stereo line-out and a microphone input. This can be set up with Mixxx in two ways:

### Practicing Mixing / Broadcasting

This setup can be used with a single audio output for speakers or headphones to practice DJing without investing in any equipment other than a computer and a set of speakers or headphones. With this configuration, use the {ref}`Pre/Main Knob <interface-head-main>` to switch back and forth between the main mix and {term}`PFL` signal. This setup cannot be used to play for a live audience because the main mix is not sent to an audio interface output. However, it can be used by radio DJs who only need to send the main mix to a broadcast audience.

1. Open {menuselection}`Preferences --> Sound Hardware`
2. Select the {guilabel}`Output` tab
3. From the {guilabel}`Headphones` drop-down menu, select your built-in audio interface, then {guilabel}`Channels 1-2`. Although this is labeled {guilabel}`Headphones`, you can also plug speakers into the output jack of your computer.
4. Depending on your audio interface, you can specify a [microphone](microphones.rst)
   a. Use your built-in microphone or connect a microphone to your computer
   b. Check that your microphone is detected by your {term}`OS <operating system>`
   c. Open the {guilabel}`Input` tab
   d. From the {guilabel}`Microphone` drop-down menu, select the input your microphone is connected to
5. Click {guilabel}`Apply` to save the changes.

### Playing for an Audience

This setup allows for playing to an audience without headphone {term}`cueing`.

![Using Mixxx with your built-in sound card](../_static/Mixxx-111-Preferences-Soundhardware.png)

1. Open {guilabel}`Preferences --> Sound Hardware`
2. Select the {guilabel}`Output` tab
3. From the {guilabel}`Main` drop-down menu, select your built-in audio interface, then {guilabel}`Channels 1-2`
4. Depending on your audio interface, you can specify a {ref}`microphone <microphones>`
   a. Use your built-in microphone or connect a microphone to your computer
   b. Check that your microphone is detected by your {term}`OS <operating system>`
   c. Open the {guilabel}`Input` tab
   d. From the {guilabel}`Microphone` drop-down menu, select the input your microphone is connected to
5. Click {guilabel}`Apply` to save the changes.

## Laptop and Splitter Cable

The cheapest way to DJ and {term}`cue` with headphones uses a stereo-to-mono DJ splitter cable (also known as a “Y cable”) plugged into the headphone jack of a laptop or other computer. This cable divides the stereo output from a single jack into two separate mono signals.

This setup allows you to start DJing without having to invest in expensive equipment. However, because the signals are in mono, you and your audience will not be able to enjoy music producers' positioning of sound in space (although many club PA systems are wired in mono anyway). Furthermore, audio interfaces built into computers are usually low quality and often pick up interference from other components of the computer.

**Using a built-in audio interface and a stereo-to-mono splitter**

1. Open {guilabel}`Preferences --> Sound Hardware`
2. Select the {guilabel}`Output` tab
3. Check that your headphones are plugged into the side of the cable with a headphones symbol and that the speakers are plugged into the side of the cable with a speaker symbol.
4. From the {guilabel}`Main` drop-down menu, select your built-in audio interface, then {guilabel}`Channel 1`
5. From the {guilabel}`Headphones` drop-down menu, select your built-in audio interface, then {guilabel}`Channel 2`
6. Click {guilabel}`Apply` to save the changes.

> **Warning:** Most splitter cables, particularly those marketed as headphone splitter cables, output the same stereo signal to two headphone jacks and will not work for this DJ setup. Also, if you use a generic stereo-to-mono splitter adapter, you may only be able to hear out of one side of your speakers and headphones. DJ splitter cables allow you to hear the same mono signal on both sides of your headphones and speakers.

## Laptop and External USB Audio Interface

![Using Mixxx together with an external audio interface](../_static/mixxx_setup_ext_audio_interface.png)

**Using two audio interfaces (built-in + external)**

1. Open {guilabel}`Preferences --> Sound Hardware`
2. Select the {guilabel}`Output` tab
3. From the {guilabel}`Main` drop-down menu, select the external audio interface, then {guilabel}`Channels 1-2`
4. From the {guilabel}`Headphones` drop-down menu, select the built-in audio interface, then {guilabel}`Channels 1-2`

**Using an external multi-channel audio interface**

1. Open {guilabel}`Preferences --> Sound Hardware`
2. Select the {guilabel}`Output` tab
3. From the {guilabel}`Main` drop-down menu, select the external audio interface, then {guilabel}`Channels 1-2`
4. From the {guilabel}`Headphones` drop-down menu, select the external audio interface, then {guilabel}`Channels 3-4`
5. Click {guilabel}`Apply` to save the changes.

## Laptop and MIDI or HID Controller

## See Also

* The {ref}`hardware-controllers` section of the {ref}`hardware` chapter has background information about controllers

### Controllers with an integrated audio interface

Many DJ controllers include an integrated *multi-channel* audio interface. A setup with this kind of controller may look like the diagram below:

![Using Mixxx together with a DJ controller and integrated audio interface](../_static/mixxx_setup_midi_integrated_audio_interface.png)

**Using a controller with an integrated multi-channel audio interface**

1. Open {guilabel}`Preferences --> Sound Hardware`
2. Select the {guilabel}`Output` tab
3. From the {guilabel}`Main` drop-down menu, select your controller's audio interface, then {guilabel}`Channels 1-2`
4. From the {guilabel}`Headphones` drop-down menu, select your controller's audio interface, then {guilabel}`Channels 3-4`
5. Click {guilabel}`Apply` to save the changes.

### Controllers without an integrated audio interface

Controllers without an integrated audio interface can be used together with a USB audio interface as depicted in the diagram below:

![Using Mixxx together with a DJ controller and external audio interface](../_static/mixxx_setup_midi_with_ext_audio_interface.png)

**Using a controller without an integrated audio interface**

1. Open {guilabel}`Preferences --> Sound Hardware`
2. Select the {guilabel}`Output` tab
3. From the {guilabel}`Main` drop-down menu, select the external audio interface, then {guilabel}`Channels 1-2`
4. From the {guilabel}`Headphones` drop-down menu, select the built-in audio interface, then {guilabel}`Channels 1-2`
5. Click {guilabel}`Apply` to save the changes.

## Laptop, External Hardware Mixer and Vinyl Control

![Using Mixxx together with turntables and external mixer](../_static/mixxx_setup_timecode_vc.png)

This setup allows DJs to use the techniques of DJing with vinyl record turntables combined with the portability and flexibility of a laptop computer. Instead of carrying crates of records or CDs, DJs can carry their entire music collection on their laptop. In addition to a laptop and headphones, this setup requires an audio interface with at least two pairs of stereo inputs and outputs as well as a pair of {term}`timecode` records.

## See Also

* Go to the chapter {term}`vinyl control` for detailed information.
