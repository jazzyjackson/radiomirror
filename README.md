# radiomirror
graph designer for filtering noise into audio-visual entities

the hall of mirrors of a fun house is an implementation of visual transforms, you have input -> transform -> output, mirrors represent a function designed to have a certain effect. The whole experience starts laying down the fact that any entity can be transformed into any other entity. 

the idea is to make playdoh of time series signals.

the interface I'm thinking of to start is a signal generator chain, processes piped together, maybe C sound if I can figure out how to pipe signals between processes

I'm imagining code snippets can be packaged as binaries that can be linked together in a node-graph interface that translates into a command line

static | filter1 -u 3 -a 34 &>2 && static | filter2 -u 34 $>3 && tee <2 <3 >1 filter3 | audio

something like that
and can also be translated to greek

So you can sort of explore effects and parameters in an experimental way

the whole time you have the RGB static trying to show as many dimensions as possible, as close as possible to a reprensative of what's going on with the noise as far as filtering out the highs and lows, 

and your composition is one of globs and flickers in high dimensional space

you can break out any greek into the code that does the work

but the greek breaks down into latex and that's how you copy paste code

I'm thinking, a change in your model forks a process with new parameters and the audio pipes are crossfaded before killing the previous model

but every line of code is stored in history, very high resolution of changes over time

As far as visualization, will have to find out whats more practical, webgl fft on audio piped from server? Is it realistic to transfer fft information - what does a frame of fft analysis look like? is it a bitmap? 

eventually if machine learning models are set loose on mimicking music, horns and drums and all that...
