---
limit: 13
---
# pcr

| Component   | Name           | Size   | Seguid                               |
|-------------|----------------|--------|--------------------------------------|
| fw primer   | p577           | 29     | lsseguid=88tnRfbdPYGncA3mXDlzes3rcFQ |
| rv primer   | p578           | 29     | lsseguid=_jCx3g-OKiK1IiEOAAObuvg3tQE |
| template    | pYPKpw         | 5603   | cdseguid=xj7evEO4h83-RGFeHu8q15tL_Qs |
| pcr product | 385bp_PCR_prod | 385    | ldseguid=2k0paIjddOVee40kQtRxzW-3ccI |

```
5GTTCTGATCCTCGAGCATCTTAAGAATTC...ACTTATGAATGTGGCAATGAGACAAGAAC3
                                 |||||||||||||||||||||||||||||
                                3tgaatacttacaccgttactctgttcttg5
5gttctgatcctcgagcatcttaagaattc3
 |||||||||||||||||||||||||||||
3CAAGACTAGGAGCTCGTAGAATTCTTAAG...TGAATACTTACACCGTTACTCTGTTCTTG5
```

Suggested program for Taq DNA polymerase.
```
|95°C|95°C               |    |tmf:63.7
|____|_____          72°C|72°C|tmr:64.1
|3min|30s  \ 58.9°C _____|____|45s/kb
|    |      \______/ 0:30|5min|GC 48%
|    |       30s         |    |385bp
```

```
>p577 lsseguid=88tnRfbdPYGncA3mXDlzes3rcFQ (fw)
gttctgatcctcgagcatcttaagaattc

>p578 lsseguid=_jCx3g-OKiK1IiEOAAObuvg3tQE (rv)
gttcttgtctcattgccacattcataagt

>pYPKpw cdseguid=xj7evEO4h83-RGFeHu8q15tL_Qs (template)
GTTCTGATCCTCGAGCATCTTAAGAATTCGTCCCACGGTTTGTCTAGAGCAGCCGACAATCTGGCCAATTTCCTGACGGGTAATTTTGATTTGCATGCCGTCCGGGTGAGTCATAGCGTCTGGTGACGTCATGCGCATGATATCTTCACAGGCGGTTTTCGCACGTACCCATGCGCTACGTTCCTGGCCCTCTTCAAACAGGCCCAGTTCGCCAATAAAATCACCCTGATTCAGATAGGAGAGGATCATTTCTTTACCCTCTTCGTCTTTGATCAGCACTGCCACAGAGCCTTTAACGATGTAGTACAGCGTTTCCGCTTTTTCACCCTGGTGAATAAGCGTGCTCTTGGATGGGTACTTATGAATGTGGCAATGAGACAAGAACCATTCGAGAGTAGGATCCGTTTGAGGTTTACCAAGTACCATAAGATCCTTAAATTTTTATTATCTAGCTAGATGATAATATTATATCAAGAATTGTACCTGAAAGCAAATAAATTTTTTATCTGGCTTAACTATGCGGCATCAGAGCAGATTGTACTGAGAGTGCACCATATGCGGTGTGAAATACCGCACAGATGCGTAAGGAGAAAATACCGCATCAGGCGCTCTTCCGCTTCCTCGCTCACTGACTCGCTGCGCTCGGTCGTTCGGCTGCGGCGAGCGGTATCAGCTCACTCAAAGGCGGTAATACGGTTATCCACAGAATCAGGGGATAACGCAGGAAAGAACATGTGAGCAAAAGGCCAGCAAAAGGCCAGGAACCGTAAAAAGGCCGCGTTGCTGGCGTTTTTCCATAGGCTCCGCCCCCCTGACGAGCATCACAAAAATCGACGCTCAAGTCAGAGGTGGCGAAACCCGACAGGACTATAAAGATACCAGGCGTTTCCCCCTGGAAGCTCCCTCGTGCGCTCTCCTGTTCCGACCCTGCCGCTTACCGGATACCTGTCCGCCTTTCTCCCTTCGGGAAGCGTGGCGCTTTCTCATAGCTCACGCTGTAGGTATCTCAGTTCGGTGTAGGTCGTTCGCTCCAAGCTGGGCTGTGTGCACGAACCCCCCGTTCAGCCCGACCGCTGCGCCTTATCCGGTAACTATCGTCTTGAGTCCAACCCGGTAAGACACGACTTATCGCCACTGGCAGCAGCCACTGGTAACAGGATTAGCAGAGCGAGGTATGTAGGCGGTGCTACAGAGTTCTTGAAGTGGTGGCCTAACTACGGCTACACTAGAAGGACAGTATTTGGTATCTGCGCTCTGCTGAAGCCAGTTACCTTCGGAAAAAGAGTTGGTAGCTCTTGATCCGGCAAACAAACCACCGCTGGTAGCGGTGGTTTTTTTGTTTGCAAGCAGCAGATTACGCGCAGAAAAAAAGGATCTCAAGAAGATCCTTTGATCTTTTCTACGGGGTCTGACGCTCAGTGGAACGAAAACTCACGTTAAGGGATTTTGGTCATGAGGGGTAATAACTGATATAATTAAATTGAAGCTCTAATTTGTGAGTTTAGTATACATGCATTTACTTATAATACAGTTTTTTAGTTTTGCTGGCCGCATCTTCTCAAATATGCTTCCCAGCCTGCTTTTCTGTAACGTTCACCCTCTACCTTAGCATCCCTTCCCTTTGCAAATAGTCCTCTTCCAACAATAATAATGTCAGATCCTGTAGAGACCACATCATCCACGGTTCTATACTGTTGACCCAATGCGTCTCCCTTGTCATCTAAACCCACACCGGGTGTCATAATCAACCAATCGTAACCTTCATCTCTTCCACCCATGTCTCTTTGAGCAATAAAGCCGATAACAAAATCTTTGTCGCTCTTCGCAATGTCAACAGTACCCTTAGTATATTCTCCAGTAGATAGGGAGCCCTTGCATGACAATTCTGCTAACATCAAAAGGCCTCTAGGTTCCTTTGTTACTTCTTCTGCCGCCTGCTTCAAACCGCTAACAATACCTGGGCCCACCACACCGTGTGCATTCGTAATGTCTGCCCATTCTGCTATTCTGTATACACCCGCAGAGTACTGCAATTTGACTGTATTACCAATGTCAGCAAATTTTCTGTCTTCGAAGAGTAAAAAATTGTACTTGGCGGATAATGCCTTTAGCGGCTTAACTGTGCCCTCCATGGAAAAATCAGTCAAAATATCCACATGTGTTTTTAGTAAACAAATTTTGGGACCTAATGCTTCAACTAACTCCAGTAATTCCTTGGTGGTACGAACATCCAATGAAGCACACAAGTTTGTTTGCTTTTCGTGCATGATATTAAATAGCTTGGCAGCAACAGGACTAGGATGAGTAGCAGCACGTTCCTTATATGTAGCTTTCGACATGATTTATCTTCGTTTCCTGCAGGTTTTTGTTCTGTGCAGTTGGGTTAAGAATACTGGGCAATTTCATGTTTCTTCAACACTACATATGCGTATATATACCAATCTAAGTCTGTGCTCCTTCCTTCGTTCTTCCTTCTGTTCGGAGATTACCGAATCAAAAAAATTTCAAAGAAACCGAAATCAAAAAAAAGAATAAAAAAAAAATGATGAATTGAATTGAAAAGCTAGCTTATCGATGATAAGCTGTCAAAGATGAGAATTAATTCCACGGACTATAGACTATACTAGATACTCCGTCTACTGTACGATACACTTCCGCTCAGGTCCTTGTCCTTTAACGAGGCCTTACCACTCTTTTGTTACTCTATTGATCCAGCTCAGCAAAGGCAGTGTGATCTAAGATTCTATCTTCGCGATGTAGTAAAACTAGCTAGACCGAGAAAGAGACTAGAAATGCAAAAGGCACTTCTACAATGGCTGCCATCATTATTATCCGATGTGACGCTGCAGCTTCTCAATGATATTCGAATACGCTTTGAGGAGATACAGCCTAATATCCGACAAACTGTTTTACAGATTTACGATCGTACTTGTTACCCATCATTGAATTTTGAACATCCGAACCTGGGAGTTTTCCCTGAAACAGATAGTATATTTGAACCTGTATAATAATATATAGTCTAGCGCTTTACGGAAGACAATGTATGTATTTCGGTTCCTGGAGAAACTATTGCATCTATTGCATAGGTAATCTTGCACGTCGCATCCCCGGTTCATTTTCTGCGTTTCCATCTTGCACTTCAATAGCATATCTTTGTTAACGAAGCATCTGTGCTTCATTTTGTAGAACAAAAATGCAACGCGAGAGCGCTAATTTTTCAAACAAAGAATCTGAGCTGCATTTTTACAGAACAGAAATGCAACGCGAAAGCGCTATTTTACCAACGAAGAATCTGTGCTTCATTTTTGTAAAACAAAAATGCAACGCGACGAGAGCGCTAATTTTTCAAACAAAGAATCTGAGCTGCATTTTTACAGAACAGAAATGCAACGCGAGAGCGCTATTTTACCAACAAAGAATCTATACTTCTTTTTTGTTCTACAAAAATGCATCCCGAGAGCGCTATTTTTCTAACAAAGCATCTTAGATTACTTTTTTTCTCCTTTGTGCGCTCTATAATGCAGTCTCTTGATAACTTTTTGCACTGTAGGTCCGTTAAGGTTAGAAGAAGGCTACTTTGGTGTCTATTTTCTCTTCCATAAAAAAAGCCTGACTCCACTTCCCGCGTTTACTGATTACTAGCGAAGCTGCGGGTGCATTTTTTCAAGATAAAGGCATCCCCGATTATATTCTATACCGATGTGGATTGCGCATACTTTGTGAACAGAAAGTGATAGCGTTGATGATTCTTCATTGGTCAGAAAATTATGAACGGTTTCTTCTATTTTGTCTCTATATACTACGTATAGGAAATGTTTACATTTTCGTATTGTTTTCGATTCACTCTATGAATAGTTCTTACTACAATTTTTTTGTCTAAAGAGTAATACTAGAGATAAACATAAAAAATGTAGAGGTCGAGTTTAGATGCAAGTTCAAGGAGCGAAAGGTGGATGGGTAGGTTATATAGGGATATAGCACAGAGATATATAGCAAAGAGATACTTTTGAGCAATGTTTGTGGAAGCGGTATTCGCAATGGGAAGCTCCACCCCGGTTGATAATCAGAAAAGCCCCAAAAACAGGAAGATTATTATCAAAAAGGATCTTCACCTAGATCCTTTTAAATTAAAAATGAAGTTTTAAATCAATCTAAAGTATATATGAGTAAACTTGGTCTGACAGTTACCAATGCTTAATCAGTGAGGCACCTATCTCAGCGATCTGTCTATTTCGTTCATCCATAGTTGCCTGACTCCCCGTCGTGTAGATAACTACGATACGGGAGCGCTTACCATCTGGCCCCAGTGCTGCAATGATACCGCGAGACCCACGCTCACCGGCTCCAGATTTATCAGCAATAAACCAGCCAGCCGGAAGGGCCGAGCGCAGAAGTGGTCCTGCAACTTTATCCGCCTCCATCCAGTCTATTAATTGTTGCCGGGAAGCTAGAGTAAGTAGTTCGCCAGTTAATAGTTTGCGCAACGTTGTTGGCATTGCTACAGGCATCGTGGTGTCACTCTCGTCGTTTGGTATGGCTTCATTCAGCTCCGGTTCCCAACGATCAAGGCGAGTTACATGATCCCCCATGTTGTGCAAAAAAGCGGTTAGCTCCTTCGGTCCTCCGATCGTTGTCAGAAGTAAGTTGGCCGCAGTGTTATCACTCATGGTTATGGCAGCACTGCATAATTCTCTTACTGTCATGCCATCCGTAAGATGCTTTTCTGTGACTGGTGAGTACTCAACCAAGTCATTCTGAGAATAGTGTATGCGGCGACCGAGTTGCTCTTGCCCGGCGTCAATACGGGATAATAGTGTATCACATAGCAGAACTTTAAAAGTGCTCATCATTGGAAAACGTTCTTCGGGGCGAAAACTCTCAAGGATCTTACCGCTGTTGAGATCCAGTTCGATGTAACCCACTCGTGCACCCAACTGATCTTCAGCATCTTTTACTTTCACCAGCGTTTCTGGGTGAGCAAAAACAGGAAGGCAAAATGCCGCAAAAAAGGGAATAAGGGCGACACGGAAATGTTGAATACTCATACTCTTCCTTTTTCAATATTATTGAAGCATTTATCAGGGTTATTGTCTCATGAGCGGATACATATTTGAATGTATTTAGAAAAATAAACAAATAGGGGTTCCGCGCACATTTCCCCGAAAAGTGCCACCTGCTAAGAAACCATTATTATCATGACATTAACCTATAAAAATAGGCGTATCACGAGGCCCTTTCGTCTCGCGCGTTTCGGTGATGACGGTGAAAACCTCTGACACATGCAGCTCCCGGAGACGGTCACAGCTTGTCTGTAAGCGGATGCCGGGAGCAGACAAGCCCGTCAGGGCGCGTCAGCGGGTGTTGGCGGGTGTCGGGGCTGGCTTAACTATGCGGCATCAGAGCAGATTGTACTGAGAGTGCACCATAGATCCTGAGGATCGGGGTGATAAATCAGTCTGCGCCACATCGGGGGAAACAAAATGGCGCGAGATCTAAAAAAAAAGGCTCCAAAAGGAGCCTTTCGCGCTACCAGGTAACGCGCCACTCCGACGGGATTAACGAGTGCCGTAAACGACGATGGTTTTACCGTGTGCGGAGATCAG

>385bp_PCR_prod ldseguid=2k0paIjddOVee40kQtRxzW-3ccI (pcr product)
gttctgatcctcgagcatcttaagaattcGTCCCACGGTTTGTCTAGAGCAGCCGACAATCTGGCCAATTTCCTGACGGGTAATTTTGATTTGCATGCCGTCCGGGTGAGTCATAGCGTCTGGTGACGTCATGCGCATGATATCTTCACAGGCGGTTTTCGCACGTACCCATGCGCTACGTTCCTGGCCCTCTTCAAACAGGCCCAGTTCGCCAATAAAATCACCCTGATTCAGATAGGAGAGGATCATTTCTTTACCCTCTTCGTCTTTGATCAGCACTGCCACAGAGCCTTTAACGATGTAGTACAGCGTTTCCGCTTTTTCACCCTGGTGAATAAGCGTGCTCTTGGATGGGTacttatgaatgtggcaatgagacaagaac
