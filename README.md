# RosettaGPCRPocketSize

Abstract: G protein-coupled receptors (GPCRs) are the largest class of drug targets and undergo substantial conformational changes in response to ligand binding. Despite recent progress in GPCR structure determination, static snapshots fail to explore the conformational space of puta-tive binding pocket geometries for small molecule ligands. In comparative modeling of GPCRs in the absence of a ligand, often a shrinking of the orthosteric hydrophobic binding pocket is ob-served. However, the exact prediction of the flexible orthosteric binding site is crucial for adequate structure-based drug discovery. In order to improve ligand docking and guide virtual screening experiments in computer-aided drug discovery, we developed RosettaGPCRPocketSize. The al-gorithm creates a conformational ensemble of biophysically realistic conformations of the GPCR binding pocket in between the TM bundle consistent with a knowledge base of expected geom-etries. Specifically, tetrahedral volume restraints are defined based on information about critical residues in the orthosteric binding site and their experimentally observed range of Cα-Cα-distances. The output of RosettaGPCRPocketSize is an ensemble of binding pocket ge-ometries which are filtered by energy to ensure biophysically likely arrangements, which can be used for docking simulations. In a benchmark set, pocket shrinkage observed in the default Ro-settaGPCR was reduced by up to 80% and the binding pocket volume range and geometric di-versity was increased. Compared to models from four different GPCR homology model databases (RosettaGPCR, GPCR-Tasser, GPCR-SSFE and GPCRdb), the here created models showed more accurate volumes of the orthosteric pocket when evaluated on the crystallographic reference structure. Furthermore, RosettaGPCRPocketSize was able to generate an improved realistic pocket distribution. However, while being superior to other homology models, the accuracy of generated model pockets was comparable to AlphaFold2 models. Furthermore, in a docking benchmark using small-molecule ligands with an increased molecular weight between 400-700 Da a higher success rate in creating native-like binding poses was observed. Additionally, Ro-settaGPCRPocketSize can be utilized to improve the pocket representation and increase the volume realistically. In summary, RosettaGPCRPocketSize can generate GPCR models with re-alistic orthosteric pocket volumes which are useful for structure-based drug discovery applications.

The here published repository of RosettaGPCRPocketSize is used for constraint file generation to build optimized pocket representation in inactive class A GPCRs
 
Associated info for Improving the modeling of extracellular ligand binding pockets in RosettaGPCR for conformational selection 
  https://www.biorxiv.org ?

If using any of the protocol, scripts or ideas please cite the article above. Thanks and happy modeling!!!

This github contains the following:

    RosettaGPCRPocketSize_Protocol_Capture.docx: Protocol capture to create your own models from the 
        input data or create constraint files for refining the binding pocket
    ADRB1_example and CXCR4_example: two examples with all the scripts and some pre-generated 
       results for comparison
    several scripts for generating a BW file, build constraint files, setup RosettaGPCR with 
       an updated XML script and calculating the volume and filtering the results
    Supporting tables with distances of selected pocket residues in all inactive
       class A GPCRs and their respective volume
