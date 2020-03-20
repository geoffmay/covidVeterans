## Questions
#### This outline of questions is divided into two phases: the “here and now” phase, and the “future-proofing” phase. 


* Here and now:
    * Can we create a facility where swabs are sent in the mail to the lab for testing? _Yes, but we need BSL-4 certification_
        * What's the fastest way to do that?
    * How do we mitigate the risk of infection from the specimens as they are transported?
        * Does BSL-4 address this?
    * What resources are needed to be able to perform testing on a large scale? _compnents are being fleshed out in tasks.md_
        * What machines?            
        * What consumable materials?
        * What materials are needed that may be scarce? _Primer is the bottleneck_
    * US has given money to Roche, their HQ is in  Germany.
        * Manufacturing units are very large, but not large enough to handle a global pandemic.
        * From a national security standpoint, would it make sense to stand up a domestic manufacturer of primers?
            * South Korea has done this.
    * How long would it take for industry to ramp up capacity to create more?
        * How much would that ramp-up cost a manufacturer?
        * How long can these materials be stored?
        * How many tests are needed per day to contain the epidemic?
          * With known rates of infection?
          * With estimated actual rates of infection?
          * By the time the program is rolled out?
    * Would it make more sense to create a government-run facility to manufacture primer?

              
* Future proofing:
    * Can we make a fully automated realtime PCR machine with the following specifications:
    * Easy to input specimens:  you simply insert a swab and press a button
      * Minimal training is needed to operate the machines beyond infection control.
    * Easy to read output:  result is unambiguous and is fast as possible
        * Is there a tradeoff between those two constraints? If so, is there sweet spot for people who are in a hurry? _A positive result can happen earlier, but negative results require the full set of cycles_
        * The machine sends an email, text message, or phone call to the patient and their doctor once an unambiguous result is obtained.
    * Information for quarantining and other infection control pertinent to the disease is delivered.
        * If security is a concern, a patient portal is available, but the patient may opt to receive the message directly after they understand the privacy implications.
    * Easy to maintain:
        * reagents are stored in cartridges that can be either refilled or swapped out quickly.
            * cartridges track:
                * what they are storing
                * how much remains
                * when they will expire
        * the machine orders replacemnt from a central facility as necessary
        * they are stored refrigerated or frozen inside the machine if that is more suitable
        * it self-cleans and disposes spent materials in the appropriate biohazard container.
            * experts can troubleshoot and change the machine settings remotely
        * Adaptable: new DNA/RNA sequences can be specified digitally and broadcast to machines around the country.
            * What reagents would need to accompany this? Can they be sent in the mail?
            * Transparent: anonymized statistics can be viewed online and allow people to track an outbreak in their neighborhood
                * Multiple vendors adhere to a standard so that data is collected easily gathered together.

* What are the costs associated with this machine?          
    * What would the R&D cost of this machine be?
    * Fixed costs of manufacturing?
    * How much would it cost to produce per machine?
    * How long would its service life be expected?
    * What kind of services would be needed to maintain the machine? How much would this cost?
    * How many machines would we need to provide coverage for the entire United States?
    * special requirements for the machine: you need a BSL-4 level facility, which can be a small room.
        * you could have a small room that is like a cold room that is BSL-4.
            * first you have to clean the sample by liquid chromatography.
                * reaction inhibitions happen because human enzymes and contaminants prevent the amplification from happening.
                * this could be automated, but they haven't yet.
                    * it is a pain. there are a lot of growth factors etc. in human serum. something like 800-1000 molecules. some of these are PCR inhibitors. around 30-40 are known, and we are pretty sure there are more that can function as inhibitors.
            * RNA is less stable than DNA.
                * so we use complementary DNA (cDNA)
                    * this part has been automated.
                * 
    * verification - positive control and negative control.
          
* Could mobile versions be developed?
    * You can in theory, not sure if they exist.
    * You need proper exhaust, etc.
    * The big thing is how you handle the waste.

* the longer RNA stays on the swab, the more quickly it will degrade. it is the most important step.
    * a stabilizing solution helps, but it should be shipped on dry ice. and as quickly as possible.

