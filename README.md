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

External modifications:

- modify in Openframeworks/graphics/ofImage.h :

      template<typename SrcType> 
      void clone(const ofImage_<SrcType> &mom); 

  Change these two lines from protected to public!

- modify ofxTextInputField.h from ofxTextInputField addon:
    
        bool    isEditing; 
        bool     isEnabled; 
          
  Change these two lines from protected to public!


- modify audiodecoderaudio.h from ofxAudioDecoder addon:
    
        //#ifdef TARGET_OS_IOS
        //#include <MobileCoreServices/MobileCoreServices.h>
        //#elif defined TARGET_OS_MAC
        #if defined TARGET_OS_MAC
          
  Comment MobileCoreServices to prevent build error
