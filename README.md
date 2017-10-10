# FRET-Analysis

Assumptions made are the following
  1.  Input requires 3 images
  2.  Each image must have 3 channels
  3.  Ch1 = donor, Ch2 = Acceptor, Ch3 = FRET (donor excite, acceptor emit)
 
FRET Gui does the following
  1.  Provides a GUI for input of three images, each with mandatory 3 channels.  GUI also provides for selection of FRET ratio method for       data analysis
  
FRET Image Analysis does the following
  1.  Captures background (bg) intensity value for each image channel (channel specific background)
  2.  Subtracts background from image intensity for each channel (channel specific subtraction)
  3.  Generates a cross talk correction coefficient from a ratio of FRET/donor and FRET/Acceptor in control images

FRET Math does the following
  1.  Uses the correction coefficients calculate the cross talk into the FRET channel of the data image (image3 in GUI)
  2.  Subtracts the crosstalk from the FRET channel of the data image
  3.  Uses whole image math to calculate a FRET ratio image from the final image, and displays ratio image plus summary data in table           format

FRET Table reports the following variables
  1.  MEAN FRET efficiency value, and SD of FRET Efficiency
  2.  Calculated correction factors, SD of correction factors
  

