# tradingDarwins
I will be using https://api.darwinex.com and Python and upload here my code in order to do realistic backtesting for Darwins.
Although Darwinex already has a tool for Darwins backtesting, my believe is that it suffers from look-ahead bias.
I will try to prove it with these snippets of code

# Function save_file(file_prefix, save_this)
This function uses pickle to store an object (save_this) in binay format. File name will be <file_prefix%Y%m%dT%H.%M%S.bin>
The function returns the string of the filename

# Function load_file(file_prefix)
This function uses pickle to load the last of the files in the current path (given by os.getcwd()) with file_prefix within its file name.
The function returns two things: the filename and the object, or -1,-1 in case of not finding files with file_prefix in the file name.

# Function get_darwins_info(force_load = False)
This function gets basic info for all darwins. Its parameter is to force download from Darwinex, or to let the function load previously downloaded data.
The function returns a list with all the darwins in it.
