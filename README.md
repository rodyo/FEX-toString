[![View String representation of any data type on File Exchange](https://www.mathworks.com/matlabcentral/images/matlab-file-exchange.svg)](https://www.mathworks.com/matlabcentral/fileexchange/38566-string-representation-of-any-data-type)

[![Donate to Rody](https://i.stack.imgur.com/bneea.png)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=4M7RMVNMKAXXQ&source=url)

# FEX-toString

TOSTRING implements an often-requested feature that is not built into MATLAB: represent some data as a string.
Supported and tested data types (of any dimension):
- double
- single
- logical
- char
- (u)int[X]
- cell
- struct
- function_handle
- user-implemented classes
The default string representation is as verbose as possible, meaning that the contents of structure fields, cell array entries, etc. are represented in fully expanded form.
S = TOSTRING(A, 'disp') produces a string representation that is identical to what the command 'disp(A)' would produce.

S = TOSTRING(A, 'compact') or S = TOSTRING(A, N) (with N a positive integer) limits the number of digits displayed in numerical arrays to either 4 ('compact') or N. A warning is issued when applied to a non-numeric array. Note that this setting also affects how enumeration classes are displayed; when this option is used, only the currently selected enumeration value will be shown, rather than the complete class.

Please report any bugs, suggestions or requests to one of the e-mail addresses mentioned in the function header.

If you consider this work useful, please consider [a donation](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=4M7RMVNMKAXXQ&source=url).
