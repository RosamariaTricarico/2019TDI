# 2019TDI

***
Project notebook: [MULTISCALE ANALYSES ON ARTERIOVENOUS FISTULA MATURATION](https://rosamariatricarico.github.io/2019TDI/FISTULA.nb.html)
***
A brief overview of a biomedical engineering project submitted to the 2019 TDI Fellowship challenge.   


***Full data-sets, R.scripts, and R Notebooks of the project are included in this repository.***   
***
   
   
      
**DATA-SETS DESCRIPTION & NOTES**       
  
**GENOMIC DATA-SET**  
*"Neutrophil.csv", "Monocyte.csv"*  
'data.frame':	26831 obs. of  100-150 variables:  
$ Gene     : Factor w/ 25193 levels "41699","41700",..: 24220 24194 7770 23654 3747 12443 13803 14186 24219 21453 ...  
 $ X31043.B : num  5.08 5.74 6.42 6.69 5.75 ...  
 $ X31044.B : num  5.1 5.57 6.44 6.62 5.67 ...  
 $ X31047.B : num  5.21 5.78 6.53 6.1 5.04 ...  
 $ X31051.B : num  5 5.66 6.92 6.68 6.01 ...  
 $ X31059.B : num  5.26 5.93 6.45 6.15 5.56 ...  
[...]    
  
Rows correspond to genes   
Columns correspond to patients  
   
"Gene" indicates the gene code listed in the fist column  
   
*Abbreviations:*    
B = baseline     
2W = 2 weeks    

**HEMODYNAMIC DATA-SETS**
*"Hemodynamics_Fistula-Artery.csv", "Hemodynamics_Fistula-Vein.csv"*  
'data.frame':	9001 obs. of  9 variables:  
 $ Patient: Factor w/ 50 levels "031072 EM","031103 PJ",..: 1 1 1 1 1 1 1 1 1 1 ...  
 $ Site   : Factor w/ 1 level "Florida": 1 1 1 1 1 1 1 1 1 1 ...  
 $ Scan   : int  1 1 1 1 1 1 1 1 1 1 ...  
 $ d.mm   : int  0 1 2 3 4 5 6 7 8 9 ...  
 $ area   : num  15.9 15.9 16.2 16.4 16.6 16.7 16.6 16.5 16.3 16.1 ...  
 $ WSSave : num  124.1 109.4 92.4 82.6 77.3 ...  
 $ WSSmax : num  179 154 128 113 106 ...  
 $ WSSGave: num  637 510 346 296 277 ...  
 $ OSI    : num  0.01 0 0 0 0 0 0 0 0 0 ...  

"Patient" indicates the patient code
"Site" indicates the location of the screening hospital   
"Scan" indicates the time of CT scan imaging (Scan == 1 #Baseline, Scan == 2 #6 weeks, Scan == 3 #6 months)     
"d mm" is distance in millimiters    
"area" is the cross sectional area in mm^2    
"WSSave" and "WSSmax" are average and maximum wall shrear stress in Pascals    
"WSSGave" is the average wall shear stress gradient in 1/Pascals    
"OSI" is the oscillatory shear index (no units)    

*Abbreviations:*    
WSS = wall shear stress    
Ave = average   
G = gradient    
  
  
**BRACHIAL ARTERY DILATION  DATA-SETS**  
*"Neutrophil_FMD_NMD data.xlsx", "Monocyte_FMD_NMD data.xlsx"*  

"original order" indicates the series number  
"PID" indicates the patient ID   
"FMD_BRACH_PRE" or "NMD_BRACH_PRE" indicates the FMD/NMD pre-fistula  
"FMD_BRACH_POST" or "NMD_BRACH_POST" indicates the FMD/NMD post-fistula  
"fmd_brach_per" indicates the percent difference between pre- and post- dilation measurements as [(PRE - POST)/PRE]*100  

*Abbreviations:*  
FMD = flow-mediated dilation   
NMD = nitroglycerin-mediated dilation   
