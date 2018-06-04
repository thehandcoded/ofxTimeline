# ofxTimeline #

Original: https://github.com/YCAMInterlab/ofxTimeline

Tested on Sierra 10.13 64-bit

Modifications (explained in commits):

- ofxTLCameraTrack.cpp
- ofxTLColorTrack.cpp
- pfxTLEmptyKeyframes.cpp
- ofxTLFlags.cpp
- ofxTLImageSequence.cpp
- ofxTLKeyframes.cpp
- ofxTLSwitches.cpp
- ofxTLTrackHeader.cpp
- ofOpenALSoundPlayer_TimelineAdditions.h

IMPORTANT!!
Also modify in Openframeworks/graphics/ofImage.h :

    template<typename SrcType> 
    void clone(const ofImage_<SrcType> &mom); 

Change these two lines from protected to public!
