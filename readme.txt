C----------------------------------------------------------------------------
C  			          circleMaps                
C----------------------------------------------------------------------------
C
C  This Pure Data patch creates "generative music" in conjunction with an 
C  electronic synthesizer.
C
C  This patch generates circle map melodies with Euclidean rhythms. The circle 
C  map values are mapped onto a scale to generate musical notes.
C  Please see http://mathworld.wolfram.com/CircleMap.html for a description of
C  circle maps.
C  
C  This patch also uses a "quantizer" modeled after Harmonaig Instruo eurorack 
C  module. https://www.modulargrid.net/e/instruo-harmonaig
C  The Instruo module is a chord generating quantizer.
C
C  Please see https://youtu.be/IMkVKST_Wgg for an example of the use of this
C  Pure Data patch.
C
C----------------------------------------------------------------------------
C  Requirements:   Pure Data <https://puredata.info/downloads/pure-data>
C----------------------------------------------------------------------------
C
Usage:  The file circleMaps.pd is the parent patch which contains the 
        rest of the modules.

              Explanation of the primary patches:
midiClockIn:  Generates bangs in sync with an external midi clock 
              from a synthesiser.
quantizer:    This patch models the Instruo by creating four note chords with various
              quality, voicing, and inversions. This patch uses the patches quality, 
              voicing, invert, setctl, and setctl2.
euclidRhythm: Creates Euclidian rhythms.              

Contributing: Any contributions to this project are welcome.

Acknowledgements: I'd like to thank Acreil for sharing his Pure Data patches. Namely; 
                  pois, rseq, and euclid, to create Euclidian rhythm patches used here.
