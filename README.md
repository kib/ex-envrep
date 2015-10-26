###About this repo
One of the more complex powershell scripts I use at work is a script initially written by Exchange MVP Steve Goodman, which was heavily modified and expanded by Ammar Hasayan.

Ammar calls it the 'Most Amazing Exchange Email Report', and I was happy using it at one point.
However, the lack of maintenance on the script has made it necessary for me to make manual edits to it to fix bugs present in it.

I've also made some adjustments based on my personal requirements.

The script as-is on this repo at this point is based on version 2.4.9 of Ammar Hasayan's script.

###Notable changes made to the script
####fixes
* [a62421f](https://github.com/kib/ex-envrep/commit/a62421f2cd07ff58f1ff73cdf74feead9ae58467): fix the scripts ability to resolve free space on mounted disks by not relying on fuzzy matching anymore.
* [9db8d1f](https://github.com/kib/ex-envrep/commit/9db8d1f64fef812cf72c083d0052e2456eb9011a): add definitions for some newer CU and SP releases
* [c1629b1](https://github.com/kib/ex-envrep/commit/c1629b13847d1775c51e44df43163281e9c67ff1): fixes the detection of rollup packages higher than 9

####changes I made for personal use
* [67b7e26](https://github.com/kib/ex-envrep/commit/67b7e2641c4e13d8f444e6c78393e86bb3d5b8ad): no local log writing
* [084ee23](https://github.com/kib/ex-envrep/commit/084ee236abfbb1c84d993d76cf3b836ef2448311): autogenerate daily report names and save them 
* [e41516e](https://github.com/kib/ex-envrep/commit/e41516eb77c1a24217d4f90c96522304dc13f788): get rid of the gaudy colours and use more manager-friendly ones (same as some other scripts i use)
* [c3cba11](https://github.com/kib/ex-envrep/commit/c3cba118df90049b7e6a88e5dd87e6b062caaa10): autoload exchange snapin when not loaded
* [fdcb2aa](https://github.com/kib/ex-envrep/commit/fdcb2aa886f1c80b0db766ce11e579d6a3dfa758): different default check values
* [28cf24a](https://github.com/kib/ex-envrep/commit/28cf24a9209bad8e1c83d070d7d0dc54c94fe535): read settings from global Settings.xml file

###references
Original script by Steve Goodman:
* blog - http://www.stevieg.org/2011/06/exchange-environment-report/
* download - https://gallery.technet.microsoft.com/exchange/Generate-Exchange-2388e7c9

Modified script by Ammar 
* blog - http://ammarhasayen.com/2013/09/24/the-most-amazing-exchange-2010-dashboard-report-script-monitor/
* download - https://gallery.technet.microsoft.com/Get-CorpEmailReport-8d708025
 
