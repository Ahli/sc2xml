# sc2xml
This is a dump of the StarCraft II game data which is all written in XML. With multiple data dumps, we can see changes between patches, e.g. via pull requests.

## Exporting game's xml data:

I wrote my own tool for this which facilitates [Zezula's CascLib](https://github.com/ladislav-zezula/CascLib):
- source code: [here in my other repo](https://github.com/Ahli/Galaxy-Observer-UI/tree/main/tools/CascExtractor/CascExtractor)
- executable for Windows: [here in my other repo](https://github.com/Ahli/Galaxy-Observer-UI/tree/main/tools/plugins/casc)
- run it with the following parameters:
    CascExtractor.exe ["Path\to\the\CASC storage"] ["*mask.txt"] ["Path\to\the\output Directory"]
    example: `CascExtractor.exe "D:\Games\StarCraft II\SC2Data" "*.xml" "D:\exportedXml"`
## Commands used to export this data:
    CascExtractor.exe "C:\Spiele\StarCraft II\SC2Data" "*.xml" ""D:\exportedXml""
    CascExtractor.exe "C:\Spiele\StarCraft II\SC2Data" "*.triggerlib" ""D:\exportedXml""
    CascExtractor.exe "C:\Spiele\StarCraft II\SC2Data" "*.galaxy" ""D:\exportedXml""
