# tradingDarwins
I will be using https://api.darwinex.com and Python and upload here my code in order to do realistic backtesting for Darwins.
Although Darwinex already has a tool for Darwins backtesting, my believe is that it suffers from look-ahead bias.
I will try to prove it with these snippets of code

# Function save_file(file_prefix, save_this)
This function uses pickle to store an object (save_this) in binay format. File name will be <file_prefix%Y%m%dT%H.%M%S.bin>
