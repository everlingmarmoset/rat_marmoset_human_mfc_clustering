Data for "Divergence of rodent and primate medial frontal cortex functional connectivity"

Naming of files:
$species:
h=human
m=marmoset
r=rat

$cluster:
c1-c4=clusters 1-4
c1-10=cluters 1-10 *For human area 24 posterior subclustering
c1-7=cluters 1-7 *For marmoset LFC clustering

$rois
Au1 = primary auditory cortex
PPC = posterior parietal cortex
S1 = primary somatosensory
M1 = primary motor
Amygdala = Amygdala
Insula = Insula
striatum = striatum
1-10 = 1-10 human area 24 posterior


Description of contained files:
$species_$cluster_map: .nii.gz seed resting state maps from each of the 4 clusters, in each species

$species_$roi: .nii.gz files of individual ROIs in respective template spaces

$species_mfc_$cluster: clustering solutions for each species

$species_$cluster_24p: .nii.gz seed resting state maps from each of the 10 area 24p subclusters

$species_$roi_24p_roi: .nii.gz files of individual ROIs for each of the 10 area 24p subclusters

$species_LFC_$cluster_LFC: .nii.gz seed resting state maps from each of the 7 marmoset LFC clusters

*Marmoset LFC clustering solutions provided in previous manuscript, see https://gin.g-node.org/everling_lab_marmosets/Marmoset_LFC_funcitonal_boundaries

*To derive fingerprints and resultant cosine similarity, please use publicly available code as follows:
1. Extract timecourse from each roi (from RS maps): https://afni.nimh.nih.gov/pub/dist/doc/program_help/3dmaskave.html

2. Normalize; in matlab: e.g., r_mfc_c1 = rescale(dlmread('r_mfc_c1.txt')

3. Calculate cosine similarity: https://www.mathworks.com/matlabcentral/fileexchange/62978-getcosinesimilarity-x-y

4. Plot fingerprint: https://www.mathworks.com/matlabcentral/fileexchange/30305-spider-rader-chart-for-multi-data

*Template anatomical files available for download through respective publications:
1. Marmoset: C. Liu, et al., A digital 3D atlas of the marmoset brain based on multi-modal MRI. Neuroimage 169, 106–116 (2018).
2. Rat: G. Paxinos, C. Watson, E. Calabrese, A. Badea, G. A. Johnson, MRI/DTI atlas of the rat brain.
3. Human: Available through AFNI: https://afni.nimh.nih.gov/AFNIAtlases

*Please contact Dr. Yuki Hori (yhori@uwo.ca) for permutation testing code, made available upon reasonable request.
