# Synth Secrets, Part 14: An Introduction To Additive Synthesis  
_Original article: [http://www.soundonsound.com/sos/jun00/articles/synthsec.htm][0]_

Every pitched sound can be thought of as a collection of individual sine waves at frequencies related to the fundamental. **Gordon Reid** introduces a powerful method of synthesis that works by manipulating these individual harmonics. This is the 14th article in a 63-part series. Read [all parts][1].

[![](http://media.soundonsound.com/sos/jun00/images/synth1_2s.gif)][2]For the past two months Synth Secrets has concentrated on frequency modulation, showing (I hope) that FM synthesis (or 'Cross Modulation' as it often used to be called) is as relevant to analogue synthesizers as it is to the digital synths that made it a household name. So now it's time to move on -- to another realm of sound creation that is normally associated only with digital synths. This month's Synth Secrets takes us into the murky world of Additive Synthesis.

**The Principle Of Additive Synthesis**

The concept underlying additive synthesis is very simple, and I can best explain it by turning all the way back to Synth Secrets Part 1 (_Sound On Sound_ May '99). In this, I showed that you could represent any waveform as a set of sine waves. For a simple harmonic oscillator, each of these sine waves has a frequency that is an integer multiple of the fundamental frequency, and we call these the 'harmonics' of the sound. Just to refresh our memory, let's take the most common synthesizer waveform -- the sawtooth wave -- as an example.

Figure 1 shows an idealised sawtooth wave. You'll never see this in nature because the universe doesn't allow physical objects such as air molecules or the cones of a 4x12 cabinet to accelerate or move infinitely quickly. Unfortunately, this is what the ideal waveform requires as it moves instantaneously from its nadir to its zenith, but we're not going to worry about that. Now, you may recall that this waveform has a simple harmonic relationship, expressed as follows: every harmonic is[![](http://media.soundonsound.com/sos/jun00/images/synth3_4s.gif)][3] present, and the amplitude of the nth harmonic is 1/n times that of the fundamental. We draw this as shown in Figure 2\.

It's important that you fully appreciate that, within limits, Figures 1 and 2 represent exactly the same thing. I have truncated the number of harmonics in Figure 2 to just nine whereas there should, in theory, be an infinite series, but neither my screen nor your copy of _SOS_ is infinitely wide, so this will have to do. If you're worried that truncating the series so severely will ruin my argument, take a look at Figure 3\. This is the waveform generated by the nine harmonics in Figure 2, and no others. It's remarkably close to the ideal sawtooth, don't you think?

Moving on, let's ask ourselves the following question. If we can represent a waveform at any given moment by describing its harmonic content at that moment, is it reasonable to assume that we can take a harmonic series and derive a unique waveform from it? Of course it is! (Well, to be precise... as long as we overlook the phase relationships of the harmonics, of course it is!) This is because, as I have already stated, the waveform and the harmonic series are simply different ways of expressing the same thing.

Armed with this knowledge, we can take our series of nine harmonics and use them to create a huge range of waveforms. For example, let's give each of the nine the same amplitude. If we now assume that these are the only harmonics within the sound, we can calculate the waveform. (See Figures 4 and 5.) As you can see, this waveform looks quite unlike the one we had before. OK, so there's a passing res[![](http://media.soundonsound.com/sos/jun00/images/synth5_6s.gif)][4]emblance, but all the 'squiggles' in the wave show that it has a much greater high-frequency content, and indeed it sounds very much brighter than the sawtooth of Figure 3\. Likewise, you could generate a passable approximation to a square wave by using your knowledge of which harmonics are present and in which quantities. (See Figures 6 and 7.)

So here is the basis of additive synthesis: because, at any given moment, you can describe any waveform in terms of the frequencies and amplitudes of its components, you can take the appropriate number of sine waves and mix them together at the appropriate frequencies and in the appropriate quantities to regenerate the waveform. Indeed, if you have a large modular synth you can easily recreate the examples shown above. All you need are nine oscillators, nine VCAs, a mixer, and some form of Gate pulse to open the amplifiers when desired (see Figure 8). Yes, it's hopelessly inefficient, but the principle holds.

**An Early Electronic Analogue Synthesizer**

If, in the analogue domain, additive synthesis were limited to monstrously over-endowed modular synths, you might think that this would be the end of our story. But it isn't, so this isn't. The choice of nine harmonics in each of these examples is not an accident, because it describes a very common analogue, additive synth. Sure, you may not think of it in this way, and you may be surprised to discover that it predates what we now think of as 'conventional' VCO-VCF-VCA analogue synthesis by about 30 years. This instrument is the Hammond Tonewheel Additive Synthesizer. Oops, sorry. I mean, it's the H[![](http://media.soundonsound.com/sos/jun00/images/synth7_8s.gif)][5]ammond Organ.

Provided that the Hammond in question is a classic 'drawbar' model, not one of the modern ones with 'tabs' for the sounds, let's dispel any doubts that you may have regarding its status as a powerful additive synthesizer. To do this, I'll describe the Hammond itself in a bit more detail...

The sound of a tonewheel organ is generated by 91 discs sitting on an axle that runs much of the length of the instrument. Each of these is shaped like an old thre'penny bit so that, when rotated in front of a pickup, it generates an electrical current that is pretty close to sinusoidal (ie. pretty close to a sine wave). If you have just one drawbar extended when you play, each key taps the output from just one disc, thus making each note a reasonably pure sine wave. (This statement ignores the distortions introduced by the valve circuitry that infests a vintage Hammond, but we're not considering such delicacies here!) If you extend a second drawbar simultaneously, you will add the output from another disc into the sound. This means that you will now have two sine waves per note. Pull out a third, and a third sine wave is added... and so on.

Figure 9 shows the classic Hammond configuration consisting of nine drawbars (see table). Each of these has nine amplitude positions (1 to 8, plus 'off') so many millions of possible combinations (more usually called 'registrations') are available. (There are a handful of Hammonds with more than nine drawbars per registration, and the spinet models have just seven on the lower manual, but we're going to ignore complications such as these.)

So there you have it: nine harmonically related pitches, each with nine possible volumes, and you can combine these in any way you choose. It's a very small leap to realise that this is, almost by definition, an additive synthesizer capable of producing millions of unique waveforms. But surely this can't be the be-all and end-all of additive synthesis? When all is said and done, the Hammond sounds, well, like an organ, not a powerful synthesizer. There's obviously something missing.

**An Analogue Additive Synthesizer**

We started this article recapping Synth Secrets 1, so now let's jump forward a few months to Synth Secrets 4 to 8\. In my discussions about filters and envelopes, I postulated that sounds will always sound static and uninteresting if they do not change in time. So this gives us a clue to today's problem: the Hammond, while a powerful signal generator, has no means to shape or contour those signals into something more involving. So let's encapsulate this in another Synth Secret:

_Organs sound like organs not because of the simplicity (or not) of their waveform gene
**Additive Synthesizers**

I first experienced additive synthesis in the late '70s during a brief encounter with a Fairlight CMI. This was a dream machine, and I fell in love with the concept of being able to manipulate the very building blocks of a sound. In the mid-'80s Kawai released the K5\. With its powerful additive engine it was, in theory, capable of all manner of sounds inaccessible from conventional analogue or digital synths. Unfortunately, the reality did not live up to the promise and the K5, while interesting, suffered from the bane of many '80s digital synths: unless treated with a great deal of love and attention it sounded sterile and uninvolving.

The final stage in this tale of additive lust brings us to the present day and my Kawai K5000S, a synth I like so much that I recently asked my producer Nick Magnus to buy one so that I didn't have to move mine between our studios. Ahhh... a happy ending!

rators, but because their sounds do not change over time._

Or, to put this another way:

_No matter how clever the method of synthesis, and no matter how complex an initial waveform may be, any timbre will sound static and 'organ-like' if it does not change in time._

One way to add interest is by applying 'effects' such as phasers, flangers, or echo units to the basic signal. Unfortunately, these do not affect the essential nature of the sound. Indeed, the Hammond has its own particular set of effects -- chorus/vibrato, reverb, and the wonderful Leslie rotary speaker -- and these help to give the instrument its distinctive sound. But you could not call these effects a method of synthesis, so we must look elsewhere if we are significantly to improve our additive synthesizer.

Consider sampling the output from a tonewheel Hammond without the chorus/vibrato, reverb, or Leslie effects. Now consider playing this sample through the contoured filters and amplifiers tha[![](http://media.soundonsound.com/sos/jun00/images/synth9s.gif)][6]t no doubt reside within your sampler. As you might imagine, the result would sound much more like a conventional synthesizer, albeit one with a more complex initial waveform than that produced by conventional oscillators. This then suggests how we can modify the 'instrument' in Figure 8 to design a more interesting additive synthesizer: simply add a time-varying filter and a time-varying amplifier after the output from the mixer (Figure 10).

However, this still is not a very interesting additive synthesizer. Indeed, if we ignore the absence of modulators (and the fact that this discussion has limited itself, so far, to sine wave oscillators) this is not much different from a multi-oscillator synth such as a Minimoog. It's just that we have nine oscillators instead of three.

Now, consider the evolution of a real sound such as a plucked string. We know from experience that this is loud and bright at the start of the note, and becomes quieter and 'darker' as time passes. So let's take this simplistic description, and see how we can modify the 'synth' in Figure 10 to recreate th[![](http://media.soundonsound.com/sos/jun00/images/synth10_11s.gif)][7]ese tonal changes more accurately. Firstly, we must assign the pitches of the oscillators to imitate the harmonic nature of the string. This is simple -- it's the 1/n harmonic series discussed many times before. Secondly, we must consider how each of these harmonics changes in time. This is also simple: we know that the sound becomes duller as time passes, so the higher-frequency harmonics must decay more rapidly than the lower ones. Thirdly, we must determine how the overall brightness and loudness of the sound changes as the note progresses, and create filter and amplifier profiles that emulate this. But hang on a minute -- if a sound can, at any instant, be determined by the relative pitches and amplitudes of its constituent harmonics, we have no need for these filters and amplifiers -- the changes in the harmonics do all the work for us. This understanding then leads us to Figure 11, which is much closer to describing how a real additive synthesizer works.

As you can see, this instrument lacks the filters and output VCA of a conventional synth. However, it is still capable of creating most of the timbres of a typical VCO-VCF-VCA configuration, plus many, many others besides.

So let's now design our simple plucked string sound. For example, let's say that Oscillator 1 produces a sine wave at the fundamental (1st harmonic) frequency, Oscillator 2 produces a sine wave at the 2nd harmonic frequency, and so on. Now, let say that Amplifier 1 causes the sound of Oscillator 1 to decay from its full level to silence in some time T, Amplifier 2 causes the sound of Oscillator 2 to decay from its maximum level to silence in half the time, T/2... and so on. These relationships mean that the higher harmonics are louder at the start, so this sound is particularly bright in the first instance, much like a plucked or hammered string. Note also that, because the higher frequencies are decaying more quickly, the sound becomes 'darker' as time passes. This is akin to a low-pass filter following a simple [![](http://media.soundonsound.com/sos/jun00/images/synth12_13s.gif)][8]AD contour with A=0 and D=T. I have shown in Figure 12 the four envelopes produced by the four contour generators.

If we now compute the waveform, we can see that the high frequencies decay quickly and that, by the time that the waveform decays to silence, only the fundamental remains. I have shown the individual sine waves in Figure 13 and the combined output in Figure 14\.

This result is much as you would expect, although in all fairness you could more easily produce it using a sawtooth oscillator and a low-pass filter controlled by a single 2-stage contour generator. But now let's ask ourselves what happens if we make individual harmonics change in less obvious ways. How about making the third and fourth harmonics start quietly, get louder and louder, and then decay quickly to zero at the end of the note? Now we have a situation where the four contours are as shown in Figure 15, and the output waveform looks like Figure 16\.

Looking at Figure 16 you can see that the waveform becomes much more complex as time passes. If you are experienced in looking at such waveforms, you can also see that the high-frequency content starts to dominate about half way through the note. This is a result that you simply can't obtain on a Minimoog, Odyssey, Prophet 5, or any other synthesizer with a single signal path. OK, you can approximate this simple example on synths with multiple signal paths (such as the Korg 800DV and, at the other end of the spectrum, the Prophet 10), but even these are limited to the simplest of such cases. In contrast, a true additive synthesizer will allow you to manipulate individually the amplitudes of 32, 64, 128, or even 256 harmonics, and that's something that no pre-patched analogue synthesizer can do.

**Fourier Synthesis And Beyond**

This method of generating a complex sound is often called Fourier synthesis. (This is in honour of Joseph Fourier, the mathematician who discovered the basis of what we now call Fourier analysis -- the mathematical method used to break sounds down into sine waves -- and Fourier synthesis -- building them back up again.) However, the more general term 'additive synthesis' does not presuppose th[![](http://media.soundonsound.com/sos/jun00/images/synth14_15s.gif)][9]at your oscillators are limited to sine waves. There is nothing stopping you from using square waves, sawtooth waves, or more complex waves such as PWM'd pulse waves or the outputs of ring modulators to create extremely complex time-varying spectra. Nevertheless, these complex waves can themselves be broken down into their constituent sine waves, so the underlying principle is always the same.

Unfortunately, if you're after complex, evolving, and involving sounds, you're going to need a lot of sine-wave oscillators in your additive synthesizer. This is why the technique is always implemented in digital technology rather than analogue. After all, in the digital realm the oscillators are merely numbers in an equation, whereas the analogue additive synthesizer will require tons (literally) of VCOs, EGs, VCAs, and mixers. And, while there's nothing stopping you from creating additive sounds using just a handful of oscillators, you're going to need dozens or even hundreds if you're going to try to recreate natural sounds that contain a lot of overtones.

But even this isn't the end of the story because, for realism, each oscillator will require modifiers that modulate its pitch and amplitude. Without these, the frequencies of the various partials remain constant relative to each other, again resulting in cheesy organ timbres. In addition, experience shows that a single LFO modulating all the harmonics simultaneously will reinforce this cheesiness, so our analogue additive synth now needs to grow to gargantuan proportions with each oscillator boasting a pitch LFO, pitch envelope, amplitude LFO, and amplitude envelope.

Furthermore, and before we become completely carried away with simply generating timbres, we should also remember that music isn't just about creating sounds, it's about playing them, preferably with some sort of expression and character. So, to all of the above, we need to add some form of control for velocity- and pressure-sensitivity, and maybe some other real-time controllers. Now you have an analogue additive synth of which you can be proud. Sure, it's going to be nigh on impossible to crowbar the thing into your bedroom studio, but you hadn't intended to sleep there anyway. Had you?

**Now Let's Get Noisy**

At this point, you may feel that your house-sized additive synth is complete. Unfortunately, it [![](http://media.soundonsound.com/sos/jun00/images/synth16s.gif)][10]isn't, and I regret to inform you that -- despite everything that I've written numerous times before -- there are many sounds that you cannot break down into the sum of their sinusoids. At this point, I should reassure you that nothing we have discussed so far is actually wrong, it's just incomplete.

Consider the sounds of orchestral instruments such as flutes and trumpets. If you have the appropriate (expensive) equipment, you can separate their sounds into their component harmonics. However, if you then subtract these harmonics from the original sound there is a residual element: noise. This noise may not be very loud or intrusive, but it's there nonetheless. Consequently, many of your synthesized sounds will remain unconvincing if they lack a little noise within them. So our additive synth needs yet another sound source -- a noise generator. Mind you, the noise produced by orchestral instruments is far from 'white' or 'pink'; it is heavily filtered by the nature of the instrument itself. So, despite everything, we need at least one filter in our additive synth. And this, of course, will need its ow[![](http://media.soundonsound.com/sos/jun00/images/synth17s.gif)][11]n contour generator to ensure that the noise colour changes realistically over time. The noise generator will also need a VCA and its associated contour generator. 

If this analysis seems a little arcane, it isn't. In fact, this extension to pure additive synthesis even has a name: if the analysis is performed beforehand it's called Spectral Modelling Synthesis. Without the signal analysis, you could just call it the 'sinusoids plus noise' model of sound generation (Figure 17).

**Don't Despair**

Despite this potential complexity, simple additive synthesis is possible on quite modest analogue synths. So is 'sinusoids plus noise' synthesis. Indeed, I guarantee that anybody playing an instrument with two or more independently tuneable oscillators (and, maybe, a noise source) has created sounds employing tuned fifths, octaves, or whatever. As soon as you have done this, you've entering the weird and wonderful world of additive synthesis. So go and find a handful of extra oscillators, and get serious. Additives can be good for you, and it's great fun, I promise. [![](http://media.soundonsound.com/images/regulars/sos_end.gif)][12]

[0]: http://www.soundonsound.com/sos/jun00/articles/synthsec.htm
[1]: /search?url=%2Fsearch&Keyword=%22synth+secrets%22&Words=All&Summary=Yes
[2]: http://media.soundonsound.com/sos/jun00/images/synth1_2.gif
[3]: http://media.soundonsound.com/sos/jun00/images/synth3_4.gif
[4]: http://media.soundonsound.com/sos/jun00/images/synth5_6.gif
[5]: http://media.soundonsound.com/sos/jun00/images/synth7_8.gif
[6]: http://media.soundonsound.com/sos/jun00/images/synth9.gif
[7]: http://media.soundonsound.com/sos/jun00/images/synth10_11.gif
[8]: http://media.soundonsound.com/sos/jun00/images/synth12_13.gif
[9]: http://media.soundonsound.com/sos/jun00/images/synth14_15.gif
[10]: http://media.soundonsound.com/sos/jun00/images/synth16.gif
[11]: http://media.soundonsound.com/sos/jun00/images/synth17.gif
[12]: http://www.soundonsound.com