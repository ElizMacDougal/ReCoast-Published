# ReCoast-Published

Uploaded scripts used to produce figures in the 2025 Restoration Ecology paper:  https://doi.org/10.1111/rec.70020.
Also available in the Dryad repository: https://datadryad.org/dataset/doi:10.5061/dryad.fbg79cp8c.

Abstract and ReadMe below are available at the Dryad repository as well.

Abstract
In two experiments, we compared the biomass of wetland plants grown in mixtures of recycled glass sand (of varying grain sizes) and dredged Mississippi River sand (dredge). Intermediate height measurements are also included in this project. For the first experiment, we grew Salix nigra, Zizaniopsis miliacea, and Sporobolus alterniflorus (Spartina alterniflora) in fine- and coarse-glass sands, dredge, and a coarse-glass/dredge mixture. For the second experiment, we grew Taxodium distichum and Schoenoplectus californicus in a revised coarse-glass blend, dredge, and a mix. For both experiments, we characterized each mixture's porosity, particle density, and bulk density. For the second experiment, we characterized the three mixtures' nutrients, metals, and pH, as well as the nutrient and metal content of S. californicus leaves grown in each mixture.

Description of the data and file structure
These data files accompany the paper "Wetland plant growth in recycled glass sand versus dredged river sand: Evaluating a new resource for coastal restoration." https://doi.org/10.1111/rec.70020. Paper authors: Elizabeth MacDougal, Bek Markel, Emily Farrer, Shehbaz Ahmad, Julie Albert, and Sunshine Van Bael. Analyses were conducted by Elizabeth MacDougal, with advising from Emily Farrer and Sunshine Van Bael. Corresponding author: Elizabeth MacDougal, emacdougal@tulane.edu

The data come from two experiments, which are described in the paper. We analyzed plant biomass, plant and soil nutrients, and soil physical properties. The RMD files here are named to indicate which data they analyze, and within each RMD file is further information about the relevant CSVs containing the data. Blank cells indicate missing data or inapplicable fields.

Files and variables

File: Biomass_Experiment1.csv
Description: 

Funding was provided by National Science Foundation Convergence Accelerator Program Award Number 2230769.

Variables
ID: IDs were assigned to mesocosms based on position in greenhouse. They range from 1-120.
Genus: Genus of the plant. Only one species per genus, so these correspond to the species referred to in the paper.
Substrate: Corresponds to soil type in the paper.
Sub: This is an abbreviation of the Substrate. F = Fine glass sand, C = Broad range coarse glass sand, M = Broad range glass/dredge mix, D = Dredge
BlockNum: Ten blocks in the experiment, each with one of each species/soil combination.
DateMeasured: Plant height, stem count, and diameter were measured before harvest. This is the date they were measured. mm/dd/yyyy
DatePlanted: All plants were originally planted on the same day, but those that died within the first two months of harvest were replaced. mm/dd/yyyy.
DateHarvested: mm/dd/yyyy
NumStems_Initial: Initial number of stems. Measured at 5cm for cutgrass.
Height_cm_Initial: Initial height in cm, measured from soil surface to tip of longest leaf (for herbaceous species) or meristem (for willow).
Diameter_mm_Initial: Initial diameter of willow in mm. Measured at Wite-Out mark placed 12cm from original soil surface.
NumStems: Number of stems. Measured at 5cm for cutgrass.
Height_cm: Height in cm, measured from soil surface to tip of longest leaf (for herbaceous species) or meristem (for willow).
Diameter_mm: Diameter of willow in mm. Measured at Wite-Out mark placed 12cm from original soil surface.
Condition: 1-5 dead to healthy.
Notes_PreHarvest: Notes that were taken prior to harvesting.
DateWetWeighed: Date that plants were weighed after harvesting and rinsing and before drying
AGWetmass_g: Mass in g of aboveground plant tissue after harvesting and before drying
BGWetmass_g: Mass in g of belowground plant tissue after harvesting and rinsing and before drying
DateAGDryWeighed: Date that aboveground tissue was weighed after it had finished drying
AGDrymass_g: Mass in g of dried aboveground tissue
DateBGDryWeighed: Date that belowground tissue was weighed after it had finished drying and extra soil had been removed from it.
BGDrymass_g: Mass in g of dried, cleaned belowground tissue. This does not count the small amount subsampled from each root mass upon harvest.
Totmass: AGDrymass_g + BGDrymass_g
Notes_Biomass: Notes taken while weighing the biomass.
Dead: Y = Yes, the plant was dead. N = No, the plant was not dead.
Exclude: Y = Yes, it should be excluded from biomass analysis. This applies to dead plants and donated plants.


File: Biomass_Experiment2.csv
Description: 

Variables
ID: IDs were assigned to mesocosms based on position in greenhouse. 60 of the original 120 mesocosms were excluded from this publication, as they were testing a separate factor.
SciName: Genus and species name
CommonName: Common name
Species: A two-letter abbreviation of the common name.
Substrate: Corresponds to soil type in the paper. G = mid-range glass mix, M = mid-range glass/dredge mix, D = dredge.
XG: N = No additional treatment.
Trt_ID: Concatenation of Substrate, XG, and ID fields.
Block: Ten blocks in the experiment, each with one of each Species/Substrate combination.
DatePlanted: mm/dd/yyyy.
Survival: Alive = Plant survived. Dead = Plant died.
DateMeasured_Initial: Initial measurements of plants, after ensuring they established. mm/dd/yyyy.
TotalStems_Initial: Number of bulrush "stems" at initial measurement. EM counted all stems, even brown. Many of the shoots had died back and measuring only the living ones would underestimate the current biomass.
Height_cm_Initial: Height from soil level to tip of longest shoot. Soil level was marked with wite out for future use. EM decided to measure longest stem even if brown. This is because many of the shoots were dying back, and measuring the longest green stem would produce an underestimate of total initial biomass.
Condition_1-5_Initial: 1- brown, 2- mostly brown, 3- half green, 4- mostly green, 5- basically all green.
Notes_InitialMeasurement: Notes taken during the initial measurements.
DateMeasured_Mid: Second measurement date. "Mid" refers to the fact that it is between initial and final measurements for the bulrush. The baldcypress were grown for longer. mm/dd/yyyy.
NumGreenStems_Mid: Number of stems with any green left.
NumBrownStems_Mid: Number of stems with no green left.
TotalStems_Mid: NumGreenStems_Mid+NumBrownStems_Mid.
Height_cm_Mid: Base of Wite-Out to tip of tallest shoot/meristem.
Diameter_mm_Mid: Only taken for baldcypress. Diameter in mm of each sample, measured just above a wite-out mark. It was not possible to measure the diameter below the rim of the pot. Thus, the wite-out mark for diameter was made at 9cm from the base wite-out that is used for the height.
Condition_1-5_Mid: 1- brown 2- mostly brown 3- half green 4- mostly green 5- basically all green
Notes_Mid: Notes at the time of midgrowth measurements.
DateMeasured_Spring: Date spring measurements were taken. mm/dd/yyyy.
NumGreenStems_Spring: Number of bulrush shoots with at least some green/Number of baldcypress branches with at least some green. This measurement involved some judgment calls. Buds on the side of the baldcypresses were counted.
NumBrownStems_Spring: Number of bulrush shoots and baldcypress branches that did not have green growth. Very dry, greyish old leaves were not counted as green for the baldcypress at this time. Only bright or dark green.
TotalStems_Spring: Total number of stems (green plus brown)
Height_cm_Spring: Height in centimeters of each sample, measured from the top of the wite-out mark to the tip of the longest green shoot or branch.
Diameter_mm_Spring: Only taken for baldcypress. Diameter in mm of each sample, measured just above a wite-out mark. It was not possible to measure the diameter below the rim of the pot. Thus, the wite-out mark for diameter was made at 9cm from the base wite-out that is used for the height.
Condition_1-5_Spring: 1- brown 2- mostly brown 3- half green 4- mostly green 5- basically all green
Notes_Spring: Notes made during spring measurements
DateMeasured_June: mm/dd/yyyy.
NumGreenStems_June:
NumBrownStems_June:
TotalStems_June:
Height_cm_June:
Diameter_mm_June:
Condition_1-5_June:
Notes_June:
DateMeasured_August: mm/dd/yyyy.
WoodyStems_August:
Height_cm_August:
Diameter_mm_August:
Condition_1-5_August:
Notes_August:
DateMeasured_September:
WoodyStems_September:
Height_cm_September:
Diameter_mm_September:
Condition_1-5_September:
Notes_September:
DateMeasured_WM: Date that the wet mass of the plant was measured. Also is the date of harvest and initial subsampling. mm/dd/yyyy.
AGWetmass_g: Mass in grams of live/green aboveground growth, immediately after harvest. This does not include the tips of shoots that had been burned by lights or had otherwise entirely dried out and gone brown. Shoots were cut off down at the rhizome where they emerged from.
AGCorrectedWetmass_g: SubtractsAGContamination_g from AGWetmass_g. Used in TotWetmassCorrected_g
BGWetmass_g: Mass in grams of live (not black and rotted) belowground growth, immediately after harvesting and rinsing. This includes rhizomes and roots, as well as shoots that never broke the surface. This measurement was taken in the greenhouse on the day of harvest. Some samples were farther processed to remove dead BG matter and substrates that weren't fully rinsed off in the greenhouse.
Notes_WM: Notes, mostly taken by the person weighing the plants. Some of the notes from lab processing were added here as well.
DeadRemoved_g: Mass in grams of black and rotted roots and portions of rhizome, removed from the initial BG sample. They do not contribute to dry weight. They were not subsampled for ITS or microscopy.
BGRinseweight_g: Some of the samples that came to the lab from the greenhouse needed further rinsing. This is the weight of those samples after they have been rinsed and after dead matter was removed. It includes the subsample weight in it. It can be used as a replacement for BGWetmass_g
BGCorrectedWetmass_g: Subtracts BGContamination_g from BGRinseweight_g, if the sample was reweighed during the initial subsampling, or from BGWetmass_g if the sample was not reweighed.
Subsample_g: The mass in g of live (not black/rotted) roots subsampled for ITS and microscopy.
BGPredryCorrected_g: Subtracts Subsample_g from BGCorrectedWetmass_g. Represents the amount of BG sample that went into the drying oven.
Subsampled_by: Several lab members and volunteers worked to subsample the roots. In case of differing methods, they are noted here. IY = Iker Ytturalde, SVB = Sunshine Van Bael, EM = Elizabeth MacDougal, and LK = Lee Kaufman
TotWetmassCorrected_g: Adds BGCorrectedWetmass_g to AGCorrectedWetmass_g to represent the total mass of each sample before drying.
TotPredryCorrected_g: Subtracts Subsample_g from TotWetmassCorrected_g. Represents the total mass that went into the drying oven, for each sample.
DateMeasured_DM_BG: Date that the dry mass of this plant was measured.
BGDrymass_Dirty_g: Mass of dried belowground matter and all substrates within the bag. This is everything that was weighed for the BGWetmass_g (or BGRinseweight if applicable).
BGDrymass_Clean_g: Mass of dried belowground matter after removing all substrates.
BGContamination_g: Difference between BGDrymass_Dirty_g and BGDrymass_Clean_g. Represents the amount of soil that was removed from the dried samples. Is used as a correction factor in a few of the wetmass columns, as the wetmass was weighed before the soil was removed from the sample.
BGDryWetRatio: Ratio between BGDrymass_Clean_g and BGPredryCorrected_g. Used to estimate the dry biomass of the subsample that was removed from the wetmass.
BGDrySubsample_Estimated_g: Multiplies Subsample_g by BGDryWetRatio to estimate the dry mass of the subsample.
BGFullDrymass_Estimated_g: Adds BGDrySubsample_Estimated_g to BGDrymass_Clean_g to estimate what the total BG drymass would be if the subsample hadn't been removed.
DateMeasured_DM_AG:
AGDrymass_Dirty_g: Mass of dried aboveground matter and all substrates within the bag. This is everything that was weighed for the AGWetmass_g (except for the samples that had been test-weighed, which lost some of their original sediment, if they had any).
AGDrymass_Clean_g: Mass of dried aboveground matter after picking it out from the substrates.
AGContamination_g: Difference between AGDrymass_Dirty_g and AGDrymass_Clean_g. Represents the amount of soil that was removed from the dried samples. Is used as a correction for AGCorrectedWetmass_g. Not available for all samples, as some were test-weighed during the drying process, and the discarded soil was not weighed at the time.
AGDryWetRatio: Ratio between AGDrymass_Clean_g and AGCorrectedWetmass_g.
TotDrymass_Estimated_g: Sum of BGFullDrymass_Estimated_g and AGDrymass_Clean_g. Estimate of the total dry biomass of the given sample, accounting for contamination and subsampling.
Notes_DM: Notes taken while weighing dried biomass.


File: MacDougal_et_al._2025_Nutrient_Analysis.Rmd
Description: This file includes all nutrient analyses described in the paper. It serves to provide more detail to those who are curious, and to help others reproduce the results. It pairs with the plant nutrient CSVs.


File: MacDougal_et_al._2025_Biomass_Analysis.Rmd
Description: This file includes all plant biomass analyses described in the paper. It serves to provide more detail to those who are curious, and to help others reproduce the results. It pairs with the plant biomass CSVs.


File: MacDougal_et_al._2025_Soil_Physical_Properties_Analysis.Rmd
Description: This file includes all soil physical properties analyses described in the paper. It serves to provide more detail to those who are curious, and to help others reproduce the results. It pairs with the soil property CSVs.


File: LSUPlantNutrients.csv
Description: See paper for methods on plant nutrient extraction

Variables
Substrate: Correlates with Soil Type in paper. D = Dredge, M = Mid-range glass/dredge mix, G = Mid-range coarse glass
Al: Aluminum (mg/kg)
As: Arsenic (mg/kg)
B : Boron (mg/kg)
Cd: Cadmium (mg/kg)
Ca : Calcium (%)
C : Carbon (%)
Cu: Copper (mg/kg)
Fe: Iron (mg/kg)
Pb: Lead (mg/kg)
Mg: Magnesium (%)
Mn: Manganese (mg/kg)
Mo : Molybdenum (mg/kg)
Ni : Nickel (mg/kg)
N : Nitrogen (%)
P : Phosphorus (%)
K: Potassium (%)
Se : Selenium (mg/kg)
Na: Sodium (mg/kg)
S : Sulfur (%)
Zn: Zinc (mg/kg)


File: Soil_Combined_LSU.csv
Description: Soil nutrient data. See paper for sampling information, including other soil properties.

Variables
Sample: Three samples were taken from each soil type of the second plant growth experiment.
SoilType: D = Dredged sand, M=1:1 mix of glass sand and dredged sand, G = glass sand
Ca_ppm: Calcium
Cu_ppm: Copper
Mg_ppm: Magnesium
pH_1to1: pH 1:1 sample to water
P_ppm: Phosphorus
K_ppm: Potassium
Na_ppm: Sodium
S_ppm: Sulfur
Zn_ppm: Zinc
OM_pct: Organic Matter
As_ppm: Arsenic
Cd_ppm: Cadmium
Pb_ppm: Lead
Ni_ppm: Nickel
Zn_HCL_ppm: Zinc extracted with HCl


File: Compaction_November.csv
Description: Compaction data for each of the mixes used in the study. See paper for specifics on grain size measurements and methods.

Variables
Sand: Describes the combination of glass sand "levels", which correspond with grain sizes the sand is sorted to after being crushed. L5 is the finest, and L2 is the coarsest we used.
SoilType: This is a shorthand for the different soil combinations used in the study. Note that the names differ from the names in the paper, but the mixes are the same. An "A" indicates it was used in the first experiment and a "B" indicates it was used in the second experiment. Fine was only used in one experiment, and Dredge was used in both.
V_SaturatedUncompressed_ml: The volume in ml of saturated, uncompressed soil.
BDUncompressed_Avg_gperml: The average bulk density in g per ml of the uncompressed soil.
MassUncompressed_Estimated_g: The estimated mass of the soil sample, given the volume and average bulk density.
StartingPosition_mm: Starting position on the die, before compression
EndingPosition_mm: Ending position on the die, after compression
SampleDisplacement_mm: Displacement of the soil sample in the die due to compression
V_SaturatedCompressed_ml: The volume in ml of the saturated compressed sand
BD_SaturatedCompressed_Estimated_gperml: The estimated bulk density in g per ml of the saturated compressed sand
Compaction: Bulk density of the compressed sand divided by the bulk density of the uncompressed sand
AveragePD: Average particle density
SaturatedCompressedPorosity: one minus the bulk density over the particle density
DieArea_cm_sq: square cm of the die area
InitialSampleHeight_cm: Initial height of each soil sample
InitialSampleVolume_ml: Initial volume of each soil sample


File: DryBulkDensity.csv
Description: This file contains the data used for the dry bulk density analyses. 

Variables
Order: Used to order the soil types
SoilType: Fine = Fine glass sand; CoarseA = Broad range coarse glass sand; CoarseB = Mid-range coarse glass sand; MixA = Broad range glass/dredge mix; MixB = Mid-range glass/dredge mix; Dredge = Dredge
Levels: Composition of each soil type. L5 is the finest glass sand size, and L2 is the largest glass sand size used in the experiment.
V_Dry_ml: Dry volume in ml used to measure bulk density
BDUncompressed_gperml: Bulk density in g per ml of uncompressed soil
BDUncompressed_gperml_Rounded: Bulk density of uncompressed soil rounded to two decimals
AverageBDDry: Average bulk density for each of the soil types
V_SaturatedCompressed_ml: Volume in ml of the saturated compressed soil
Mass_SaturatedCompressed_g: Mass in g of the saturated compressed soil
ProportionWater: Proportion of the sample that is water
WeightWater_Calculated_g: Calculated weight in g of water
Mass_CompressedSoil_Calculated_g: Calculated mass in g of the compressed soil
BD_SatCompEst_gperml: Estimated bulk density in g per ml of the saturated compressed soil
BD_SatCompEst_Rounded1: Estimated bulk density of the saturated compressed soil, rounded to two decimal places
BDSatCompEst_gperml_Est2: Estimated bulk density in g per ml of the saturated compressed soil, using a different method for estimation
BD_SatCompEst_Rounded2: The second estimate method, rounded to two decimal places.


File: Porosity.csv
Description: Data used for porosity analyses of the different substrates. Five samples were tested from each soil type used in the experiment. See paper for methods.

Variables
Substrate: Fine = Fine glass sand; CoarseA = Broad range coarse glass sand; CoarseB = Mid-range coarse glass sand; MixA = Broad range glass/dredge mix; MixB = Mid-range glass/dredge mix; Dredge = Dredge
Mass of sand (g): Mass of sand used for the test
Initial Volume of water (ml): Initial volume of water in graduated cylinder
Final Volume of water (ml): Water level in graduated cylinder after sand sample was added
Volume of sand (ml): Volume of sand that was added to the graduated cylinder
Bulk Density(g/ml): Bulk density of the sand, calculated from the sample mass over the initial sample volume.
ParticleDensity_gperml: The density of the particles in the sand, calculated from the sample mass over the volume of water displaced.
Porosity: 1- soil bulk density/soil particle density

Code/software
The CSVs can be viewed via many free programs, including LibreOffice or Google Sheets.

The RMDs can be viewed using RStudio, and contain code written in R, both of which are free. To run the RMD scripts, a user would need to download the scripts and CSVs, Install R, and change the filepaths in the RMD files to match the new location of these files on their own device. Each RMD file should include all libraries needed as well as comments describing what they are needed for.
