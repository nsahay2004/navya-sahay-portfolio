Project: https://devpost.com/software/eye-based-communication ; 
https://github.com/kana820/Blink-147 

Description: Total paralysis patients often rely on eye-based communication, using different eye movements 
to relay basic needs such as food and personal well-being.To accurately translate their messages and make 
this form of communication more accessible, we propose an attention-based CNN model to first detect eye 
location within facial images. The CNNs determine and classify specific eye movements relevant to a 
predefined eye alphabet, “up”, “left”, “right”, and “down” within the localized eye images.Our goal is to 
improve on Blink-To-Live, an eye-tracking system based on facial landmark detection (DLib) designed by Ezzat et al. 
2023, to classify eye movements with greater accuracy across a more diverse audience. The paper’s objectives 
are to develop a computational eye-based communication system for patients with motor neuron disorders, 
especially in low-income countries. This architecture, Blink-To-Live, is not software or hardware-specific, 
serving as a cost-efficient alternative to comparable sensor-based systems.Blink-To-Live establishes an 
eye gesture alphabet such that speech-impaired patients are able to express their basic needs.

We chose this paper as we are all interested in nonverbal communication and how technology could universalize 
what would otherwise be marginalized languages. We were impressed by the ingenuity of this paper, and we were 
inspired by the use of deep learning in medical technology. However, when we tried the original Blink-to-Live model 
on our own faces, we noticed that Blink to Live was unable to recognize diverse shapes of eyes and classify them 
accurately because of the aspect ratio-based analysis of eye images. Thus, we hoped to use a more diverse dataset and 
a simpler CNN-based model, rather than the computer vision library used in the paper, to improve the performance 
of eye language recognition models for a broader range of users.  
