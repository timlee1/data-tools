% UTF8-SCRIPT(1)
% Clark Grubb
% February 14, 2015


# NAME

utf8-script - tally UTF-8 encoded characters by general category

# SYNOPSIS

utf8-script [-l|\--long-names] [-c|\--count-ascii|-s|\--skip-ascii]

# DESCRIPTION

Tally the UTF-8 encoded characters in the standard input stream by general category.

     Abbr  Long                    Description
     ---   ----                    -----------
     Lu    Uppercase_Letter        an uppercase letter
     Ll    Lowercase_Letter        a lowercase letter
     Lt    Titlecase_Letter        a digraphic character, with first part uppercase
     LC    Cased_Letter            Lu | Ll | Lt
     Lm    Modifier_Letter         a modifier letter
     Lo    Other_Letter            other letters, including syllables and ideographs
     L     Letter                  Lu | Ll | Lt | Lm | Lo
     Mn    Nonspacing_Mark         a nonspacing combining mark (zero advance width)
     Mc    Spacing_Mark            a spacing combining mark (positive advance width)
     Me    Enclosing_Mark          an enclosing combining mark
     M     Mark                    Mn | Mc | Me
     Nd    Decimal_Number          a decimal digit
     Nl    Letter_Number           a letterlike numeric character
     No    Other_Number            a numeric character of other type
     N     Number                  Nd | Nl | No
     Pc    Connector_Punctuation   a connecting punctuation mark, like a tie
     Pd    Dash_Punctuation        a dash or hyphen punctuation mark
     Ps    Open_Punctuation        an opening punctuation mark (of a pair)
     Pe    Close_Punctuation       a closing punctuation mark (of a pair)
     Pi    Initial_Punctuation     an initial quotation mark
     Pf    Final_Punctuation       a final quotation mark
     Po    Other_Punctuation       a punctuation mark of other type
     P     Punctuation             Pc | Pd | Ps | Pe | Pi | Pf | Po
     Sm    Math_Symbol             a symbol of mathematical use
     Sc    Currency_Symbol         a currency sign
     Sk    Modifier_Symbol         a non-letterlike modifier symbol
     So    Other_Symbol            a symbol of other type
     S     Symbol                  Sm | Sc | Sk | So
     Zs    Space_Separator         a space character (of various non-zero widths)
     Zl    Line_Separator          U+2028 LINE SEPARATOR only
     Zp    Paragraph_Separator     U+2029 PARAGRAPH SEPARATOR only
     Z     Separator               Zs | Zl | Zp
     Cc    Control                 a C0 or C1 control code
     Cf    Format                  a format control character
     Cs    Surrogate               a surrogate code point
     Co    Private_Use             a private-use character
     Cn    Unassigned              a reserved unassigned code point or a noncharacter
     C     Other 	               Cc | Cf | Cs | Co | Cn

# OPTIONS

-c, \--count-ascii
: treat ASCII characters as a separate general category called "ASCII".

-l, \--long-names
: use long names for the general categories instead of the two character abbreviations.

-s, \--skip-ascii
: skip ASCII characters.  Only characters with Unicode point U+0080 and higher are counted.

# SEE ALSO

http://unicode.org/reports/tr44/#General_Category_Values

