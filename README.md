# xml2struct
Semi-optimized utility for converting an xml document to a MATLAB structure

This project utilizes pugixml, an XML parser for C++ found here: https://github.com/zeux/pugixml

This project was created in order to facilitate time-efficient parsing of large XML files on windows based systems. 

This utility attempts to remain compatible with the MATLAB implementation found here: https://www.mathworks.com/matlabcentral/fileexchange/28518-xml2struct

This utility has been tested in MATLAB using the MinGW compiler.

In order for the project to be compiled, the pugixml utility source needs to be downloaded. As of right now, the necessary files are, pugiconfig.hpp, pugixml.cpp, and pugixml.hpp.

Assuming a proper compiler configuration, the xml2struct can be compiled by `mex xml2struct.cpp pugixml.cpp`. The result will be a xml2struct.mex file that can be used by, `struct = xml2struct('*.xml');`.

