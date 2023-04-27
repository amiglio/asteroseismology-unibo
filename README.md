# asteroseismology-unibo

in this repo I will upload material useful for the computer-lab component of the module "Advanced stellar evolution and Asteroseismology"


##### MESA tips:

- If you wish to assign different names to the various runs (e.g. changing, mass, chemical composition, ...) you can set the file names adding these lines in the &controls section in the inlist_project file:

		star_history_name =    'NAME.track'
		profiles_index_name =  'NAME.index'
		profile_data_prefix =  'NAME_n'


- If you wish to save the graphical windows as png files, for each of them you can set the file_flag to .true. and specify prefixes for filenames etc

		TRho_Profile_file_dir = 'png'
		TRho_Profile_file_flag = .true.
		TRho_Profile_file_prefix = 'trho_profile_'
		TRho_Profile_file_interval = 5 ! output when mod(model_number,TRho_Profile_file_interval)==0
		TRho_Profile_file_width = -1 ! (inches) negative means use same value as for window
		TRho_Profile_file_aspect_ratio = -1 ! negative means use same value as for 
	
files will be saved in a folder named `png`
