BCC: Bash Currency Converter
Simple up-to-date currency converter in bash.




Dependencies: netcat, bc, printf, awk

Add to your /usr/bin, alias in your .bashrc or whatever
Usage: bcc sourceCurrency destinationCurrency amount
Examples:
 	bcc AUD USD 10
 	bcc GBP LAK 10
 	bcc NOK JPY 7463
 	bcc --list | grep "United States"
 	bcc --

 Issues:
 	Doesn't use correct source or destination currency symbols (only uses $ at the moment)
 	4 d.p. is a little ugly
 	Relies on 3 letter country codes, but you can search them using grep
	Probably horrendously ineffecient
	My args parsing is awful. Apologies
	The country code list is quite big...