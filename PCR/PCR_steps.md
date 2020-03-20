## Steps to perform realtime polymerase chain reaction (PCR)

* guiding principles
    * you have to be careful, it's easy to mess up.
    * there are 3 considerations when you're deciding how to proceed:
        * what is the gold standard?
        * what is the risk of false positive?
        * what is the risk of false negative?
            * this one is the disaster in a pandemic.


* broadly there are 3 steps:
    * isolate the mRNA
    * create complementary DNA
    * amplify the DNA
* mRNA isolation (cleaning)
    * sequential, centrifuging at basically every step (8000rpm for 15 seconds)
        * lyse the viral capsules
            * What reagent and how much?
        * then add a buffer with phenol to get rid of the protein
            * How much?
            * centrifuge to remove proteins
        * remove DNA using ethanol
            * how much?
            * centrifuge
        * now you're left with RNA
            * dump it on a column that binds RNA (small, maybe 1/2 inch)
                * qiagen is the big manufacturer. they make the best thing that binds RNA and blow everyone else out of the water.
        * now RNA is bound to resin.
            * elute with water, this takes the rna off the resin
                * centrifuge the column to pull the RNA off
            * you want it "enriched," which means you eluted with as little water as possible
* create complementary DNA (cDNA) using RNA as a template.
    * this happens at 37 degrees C for 1 to 2 hours.
    * need 10-50ng of RNA, depending on the amount it's expressed
        * (mRNA that is expressed more by the virus will take up a greater proportion of the mRNA in your vial)
        * you (hopefully) have much more than that in your sample (say 1.5 ug).
    * transfer the appropriate amount of solution to your next vial 
    * you can target multiple genes, but it's best to do each one in a separate vial
        * [spectrophotometer](https://en.wikipedia.org/wiki/Nucleic_acid_quantitation) is used to test for concentration. 
            * 260nm light is absorbed by mRNA and DNA
            * 280nm light is not
            * you want a ratio of somewhere around between 1.8 and 2.2.
            * gradually add mRNA until you get it.
                * could you start with a lower volume of solvent in case you're starting with very little mRNA?
            * don't proceed if you can't achieve this concentration. tell the patient you need another, better sample.
        * save the rest of your RNA at in -20 degrees C for shipment (on dry ice) back to the central lab
            * at -80 it's good for 3-4 years
        * combine your mRNA with:
            * DNA nucleotides 
                * chosen in quantities based on the primer 
            * reverse transcriptase 
            * a universal set of primers
        * let simmer for 1-2 hours at 37 degrees C.
            * now you have cDNA.
            * save whatever you don't amplify for analysis of mRNA expression
                * they should be shipped back on dry ice, and stored at -20 is fine
                    * because DNA is more stable than RNA.
* now do real-time PCR
    * you are going to cause taq polymerase to make lots of copies of the cDNA
    * add your buffer than contains primers and taq polymerase
        * taq polymerase will bind and make a copy of the DNA when it's warm and release when it's cool
        * different primers have different annealing temperatures.
            * e.g. ~60.5 vs. 62 degrees Celsius.
            * that level of precision is important.
    * taq polymerase starts at the primer and creates a copy of your chosen cDNA gene.
        * there can be quality problems with different taq polymerases.
            * type 1 always works.
                * there are still differnet subtypes: genetically engineered, chemically syntehsized, etc.
    * a separate vial for every primer is BETTER.
        * otherwise the most abundantly expressed primer will exhauset the nucleotides of the others.
    * you will do up to 40 cycles of heating and cooling.
        * each cycle takes 2-3 minutes
        * most machines run these in series (!)
            * because all the cycles are the same, you could have a larger chamber that runs cycles in parallel
            * the robot just needs to keep track of when each vial went in and needs to come out  
    * after your last cycle, you attach a primer that has fluorescein dye.
        * with realtime PCA, all your primers have the dye and they get measured after every cycle.
            * (how do you detect only the dye that is bound to DNA?)
        * a photodetector will register be brighter if you started with a higher concentration.
            * this will rise exponentially as you double the amount of target DNA you have each cycle.
        * you can report your result if you detect something at an eariler cycle
            * if you have excess capacity, you can continue your cycles to watch your curve behave properly
        * lower number of cycles => higher starting concentration.
        * repeat the test if you only get it at a late cylce.
        * negative control is run separately.
            * minus all reagents
            * positive result means you somehow got mRNA from somwhere else contaminating your sample.
        * positive control is known cDNA (e.g. coronavirus cDNA)
            * no reaction => you probably missed some taq transcriptase inhibitors.
                * retry with leftover mRNA 
                    * try using e.g. more phenol rinses?


