# Experiments

 A collection of cognitive / behavioral tasks, mostly implemented in [OpenSesame](https://osdoc.cogsci.nl/), for research in Psychology, Cognitive, and Integrative Neuroscience.

  All the scripts are work in progress unless otherwise specified, and even then they may not be suitable for your research purposes. You are welcome to use and modify them according to your needs. 
  
  
# List of Experiments

# Final Form

##  01 Blini et al., *Cortex*, 2018 

Blini, E., Tilikete, C., Farnè, A. & Hadj-Bouziane, F. (2018). Probing the role of the vestibular system in motivation and reward-based attention. *Cortex*, 103, 82-99. [(link)](https://www.sciencedirect.com/science/article/pii/S0010945218300583?via%3Dihub)

In this experiment  we used Galvanic Vestibular Stimulation (GVS) to assess whether a vestibular perturbation affects motivational processing. We found that, indeed, GVS decreases the sensitivity to monetary rewards.

There are three scripts:

  1) 01 SVV: participants are asked to align visual segments to the perceived vertical. The task should be administered in a dark room and with a round paper cover for the monitor screen in order to minimize external cues of verticality. The perception of verticality is affected by a vestibular stimulation (or vestibular disorders). 
  
  2) 02 PosnerReward: as the name suggest this is a very classic Posner (discrimination) task (e.g. Posner, 1980), with exogenous unpredictive cues that are colored as a function of the reward at stake. There is a feedback on a trial basis.
  
  3) 03 Questionnaire: this is simply used to present an ad-hoc questionnaire with several follow-up questions for the experiment. This is not achieved via the OpenSesame forms but rather through an analogue visual scale requiring a mouse response plus a confirmation via keyboard.


##  02 Blini et al., *Cortex*, 2020

Blini, E., Tilikete, C., Chelazzi, L., Farnè, A., & Hadj-Bouziane, F. (2020). The role of the vestibular system in value attribution to positive and negative reinforcers. *Cortex*, 133, 215-235. [link](https://www.sciencedirect.com/science/article/pii/S0010945220303427?via%3Dihub)

This may be regarded as a follow up of the previous study. Like the previous study, this was a [registered report](https://www.cos.io/initiatives/registered-reports) attempting to relate vestibular perturbations and motivational processing. We have found some weak evidence for GVS to further increase the processing of losses, as suggested by even larger interference costs in a task evoking conflict (Eriksen's flankers task). Results were, however, overall ambiguous, and suggest that much more research is needed to better understand the link between the vestibular system and motivation.

There are three scripts (two of them are very similar to those above or present minor edits):

  1) 01 SVV: participants are asked to align visual segments to the perceived vertical. The task should be administered in a dark room and with a round paper cover for the monitor screen in order to minimize external cues of verticality. The perception of verticality is affected by a vestibular stimulation (or vestibular disorders). 
  
  2) 02 FT task: a task based on Eriksen's flankers task (e.g. Eriksen, 1995; Eriksen & Eriksen, 1974) which includes motivational information (neutral trials, potential losses, potential gains) in the form of colored distractors (arrows).
  
  3) 03 Questionnaire: this is simply used to present an ad-hoc questionnaire with several follow-up questions for the experiment. This is not achieved via the OpenSesame forms but rather through an analogue visual scale requiring a mouse response plus a confirmation via keyboard.

# Work in progress

Files uploaded here are likely stable but still under active testing/evaluation and subject to change. They mostly include scripts that are meant to be used with concurrent eye-tracking, as this is what I am trying to do in these weird covid-fested times.

**Important Note.** I have access to a **Tobii Spectrum eye-tracker**, and that's what I am using as a reference in the scripts. However, please note that Tobii (up to today) does not provide Python bindings for Python 3.7, so I had to switch back to OpenSesame with Python version 2.7. You need this version and the tobii_research bindings imported from pip to use the scripts. You will probably want to modify these scripts in order to match the needs of your eyetracker (e.g., serial number...). 

## Attention to Nicotine Related Stimuli

Here I am trying to validate tasks capable to robustly highlight altered, possibly enhanced attention to Nicotine-Related Stimuli. Ideally the goal is to test differences between groups of smokers, former smokers, and non-smokers. Both overt (eye-movements) and covert (RTs) indices will be obtained.

  1) The Dot Probe Task is a classic version (Posner-like if you wish). Images of nicotine-related or matched (at best) control images are presented as lateral cues before the onset of a target (a landholt C) on the same or opposite side.
  
  2) The Passive Viewing task is mostly used for pupillometry and, as the name suggest, it is a very simple task consisting of the passive presentation of stimuli (nicotine-related vs. controls) with an occasional rare stimulus to detect (in order to keep participants as engaged as possible). 

## Gaze-contingent eyetracking scripts

As the name suggest, this script monitors eye movements online and adaptively change the given feedback. This is meant to be used with patients with visual/attentional deficits (but not only them of course) as a sort of visual search task, in which the target is invisible, to better characterize their oculomotor behavior. 
In the *INIT* part of the file several parameters can be adapted according to the required feedback. For example, an auditory sound may play until the participant is fixating the target, and more loudly so the more participants are fixating farther away from it, or with a different pitch. The reverse is also possible (e.g., the sound is only presented on the sweet spot). Optional options for visual aids and debugging are also outlined in the **INIT** part.





  
  
  
  

