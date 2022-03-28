#Analysis of further processing paths of biogas for mobility purposes
This project is part of the master thesis 'Analysis and evaluation of different technologies for the further processing of biogas for the use in the mobility sector'. 
It should provide an analysis of the processing paths of biogas upgrading, steam reforming, and Fischer-Tropsch synthesis to create fuels for mobility purposes.

##Instructions
1. The data for the biogas plants used for analysis are taken from the 'Biogas-Messprogramm III' [1]. Here, all required data should be found to add a new biogas plant into the database. This can be done by using the function SQLiteBiogasPlant.insert_biogas_plant(). If there is not sufficient data in [1], an estimation has to be made. The ghg-avoidance cannot be found in [1], but instead it has to be calculated using RED II [2].
2. After putting a biogas plant into the database, an instance of this biogas plant has to be created using the function SQLiteBiogasPlant.set_biogas_plant()
3. The instance can be used for the technical and economical analysis of the biogas plant for the different processing paths, an example for biogas plant 11 from [1] is given in ReferenceBiogasPlant.py
4. If the parameters for the analysis need to be adjusted, this can be done in PARAMETER.py
5. SciPy needs to be installed to enable the interpolation

##Analysis data basis
###Biogas upgrading
The technical analysis for the biomethane yield estimation is based on 'Selection of appropriate biogas upgrading technology' [3].
The economical analysis is based upon 'Effiziente-Mikro-Biogasaufbereitungsanlagen (eMikroBGAA)' [4].
Furthermore, for the calculation of the biomethane distribution, the report 'Wirtschaftliche Chancen der Biogas-Versorgung netzferner Gas-Tankstellen gegenüber konventioneller Erdgas-Versorgung' [5] was used.
###Steam reforming
The estimation for the hydrogen yield is based on 'Techno-ökonomische Analyse der regenerativen Produktion von Wasserstoff für den Einsatz in Fahrzeugen' [6].
The technical analysis is based on 'Scenario-Based Techno-Economic Analysis of Steam Methane Reforming Process for Hydrogen Production' [7].
For the economical analysis the report 'Evaluierung der Verfahren und Technologien für die Bereitstellung von Wasserstoff auf Basis von Biomasse' [8] was used.
###Fischer-Tropsch synthesis
The technical as well as the economical analysis is mainly based on 'Is the Fischer-Tropsch Conversion of Biogas-Derived Syngas to Liquid Fuels Feasible at Atmospheric Pressue?' [9].

Further information about the literature used is illustrated in the thesis.

[1] Fachagentur Nachwachsende Rohstoffe e.V. (FNR). Biogas-Messprogramm III.
1st edition, 2021.
URL: https://www.fnr.de/fileadmin/Projekte/2021/Mediathek/bmp_2020_web_stand2021.pdf

[2] Europäisches Parlament und Rat. Richtlinie (EU) 2018/2001 zur Förderung
der Nutzung von Energie aus erneuerbaren Quellen. URL: https://eur-lex.europa.eu/legal-content/DE/TXT/PDF/?uri=CELEX:32018L2001

[3] Qie Sun, Hailong Li, Jinying Yan, Longcheng Liu, Zhixin Yu, and Xinhai Yu.
Selection of appropriate biogas upgrading technology-a review of biogas cleaning,
upgrading and utilisation, 2015. Renewable and Sustainable Energy Reviews,
Vol. 51, p. 521-532. 

[4] Gert Müller-Syring Ronny Erler Sven Jakob Michael Beil, Jaqueline Daniel-
Gromke. Effiziente-Mikro-Biogasaufbereitungsanlagen (eMikroBGAA), February 2019. Endbericht 2/2019. FNR Verbundvorhaben von Fraunhofer
IEE,DBFZ, DBI und dena. URL: https://www.fnr.de/ftp/pdf/berichte/22402411.pdf

[5] C. Gikopoulos, M. Dos Santos, L. Targyik-Kumer, R. Adler, E. Klein, D. Hornbachner, and V. Kryvoruchko. Wirtschaftliche Chancen der Biogas-Versorgung
netzferner Gas-Tankstellengegen gegenüber konventioneller Erdgas-Versorgung. Bundesministerium für Verkehr, Innovation und Energie, 2009.
URL: https://nachhaltigwirtschaften.at/resources/edz_pdf/0954_biogastankstellen_edz-814153.pdf

[6] Angela Miltner. Techno- ökonomische Analyse der regenerativen Produktion von
Wasserstoff für den Einsatz in Fahrzeugen. PhD thesis, Technische Universität
Wien, 2010.

[7] Shinje Lee, Hyun Seung Kim, Junhyung Park, Boo Min Kang, Churl-Hee Cho,
Hankwon Lim, and Wangyun Won. Scenario-Based Techno-Economic Analysis
of Steam Methane Reforming Process for Hydrogen Production, 2021. Applied
Sciences, Vol. 11, No. 13

[8] Konstantin Zech, Elias Grasemann, Katja Oehmichen, Isabel Kiendl, Ralf
Schmersahl, Stefan Rönsch, Michael Seiffert, Franziska Müller-Langer, Werner
Weindorf, Simon Funke, Julia Michaelis, and Martin Wietschel. Evaluierung
der Verfahren und Technologien für die Bereitstellung von Wasserstoff auf Ba-
sis von Biomasse. Deutsches Biomasseforschungszentrum (DBFZ), 2014.
URL: https://www.dbfz.de/fileadmin/user_upload/Referenzen/DBFZ_Reports/DBFZ_Report_19.pdf

[9] Rawan Hakawati, Beatrice Smyth, Helen Daly, Geoffrey McCullough, and David
Rooney. Is the Fischer-Tropsch Conversion of Biogas-Derived Syngas to Liquid
Fuels Feasible at Atmospheric Pressure?, 2019. Energies, Vol. 12, No. 6.